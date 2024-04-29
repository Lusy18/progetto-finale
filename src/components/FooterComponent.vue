<template>
    <section class="dizme_section ">
        <div class="copyright">
            <div class="container">
                <div class="inner">
                    <div class="left">
                        <p>Developed with love by <a href="https://themeforest.net/user/marketify"
                                target="_blank">Marketify</a> &copy; 2022</p>
                    </div>
                    <div class="right">
                        <ul>
                            <li><a href="#">Terms &amp; Condition</a></li>
                            <li><a href="#">Privacy Policy</a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>

        <div id="myBar" :style="{ width: scrollPercentage + '%' }"></div>
        <!-- Pulsante per scorrere verso l'alto -->




        <div class="progressbar animate">
            <a href="#" @click.prevent="scrollToTop">
                <span class="text" style="bottom: 150.75px;">To Top</span>
            </a>
            <span class="line" style="height: 7,91497%;"></span>
        </div>

        
        <div class="mouse-cursor cursor-outer"></div>
        <div class="mouse-cursor cursor-inner"></div>
        <div class="custom-cursor"></div>
      







    </section>







</template>


<script>


export default {
    name: "FooterComponent",



    data() {
        return {
            scrollPercentage: 0,

        };
    },


    mounted() {
        window.addEventListener('scroll', this.handleScroll);
        // cursore
        this.addCursorAnimation();
    },
    beforeUnmount() {
        window.removeEventListener('scroll', this.handleScroll);
    },
    methods: {
        handleScroll() {
            const winScroll = document.body.scrollTop || document.documentElement.scrollTop;
            const height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
            this.scrollPercentage = (winScroll / height) * 100;
        },
        scrollToTop() {
            window.scrollTo({ top: 0, behavior: 'smooth' });
        },

        // cursore
        addCursorAnimation() {
            const cursorOuter = document.querySelector('.cursor-outer');
            const cursorInner = document.querySelector('.cursor-inner');
            
            
            document.addEventListener('mousemove', (e) => {
                const x = e.clientX;
                const y = e.clientY;

                cursorOuter.style.left = x + 'px';
                cursorOuter.style.top = y + 'px';
                cursorInner.style.left = x + 'px';
                cursorInner.style.top = y + 'px';

            
            });

        }


    }
}









</script>

<style scoped>

.copyright {
    width: 100%;
    height: auto;
    background-color: #3f4453;
    padding: 57px 0 61px
}

.copyright .inner {
    width: 100%;
    height: auto;
    display: flex;
    align-items: center;
    justify-content: space-between
}

.copyright .left p {
    font-size: 18px;
    color: #b9b5c9
}

.copyright .left a {
    text-decoration: none;
    color: #b9b5c9;
    font-weight: 700;
    -webkit-transition: all .3s ease;
    -moz-transition: all .3s ease;
    -ms-transition: all .3s ease;
    -o-transition: all .3s ease;
    transition: all .3s ease
}

.copyright .left a:hover {
    color: #f75023
}

.copyright .right ul {
    margin: 0;
    list-style-type: none
}

.copyright .right ul li {
    margin: 0 42px 0 0;
    display: inline-block
}

.copyright .right ul li:last-child {
    margin-right: 0
}

.copyright .right ul li a {
    text-decoration: none;
    color: #b9b5c9;
    font-size: 18px;
    -webkit-transition: all .3s ease;
    -moz-transition: all .3s ease;
    -ms-transition: all .3s ease;
    -o-transition: all .3s ease;
    transition: all .3s ease
}

.copyright .right ul li a:hover {
    color: #f75023
}



.progressbar {
    position: fixed;
    height: 100px;
    width: 1px;
    bottom: 25px;
    right: -25px;
    background-color: grey;
   
}

.progressbar.animate {
    right: 25px;
    animation: 2s linear infinite; /* Aggiunge l'animazione */
}

.progressbar .line {
    /* position: absolute; */
    width: 3px;
    height: auto;
    background-color: grey;

}

.progressbar .text {
    position: absolute;
    bottom: 100px;
    left: 0;
    font-size: 13px;
    transform: rotateZ(90deg);
    text-transform: uppercase;
    transform-origin: left;
    white-space: nowrap
}

.progressbar a {
    text-decoration: none;
    color: white
}




/* cursore syle */


.mouse-cursor {
    position: fixed;
    left: 0;
    top: 0;
    pointer-events: none;
    border-radius: 50%;
    -webkit-transform: translateZ(0);
    transform: translateZ(0);
   
}

.cursor-outer {
    margin-left: -15px;
    margin-top: -15px;
    width: 30px;
    height: 30px;
    border: 2px solid #f75023;
    -webkit-box-sizing: border-box;
    box-sizing: border-box;
    z-index: 100;
    opacity: .5;
    -webkit-transition: width .09s ease-in-out, height .09s ease-in-out, margin .09s ease-in-out, opacity .09s ease-in-out;
    transition: width .09s ease-in-out, height .09s ease-in-out, margin .09s ease-in-out, opacity .09s ease-in-out; 
    
}

.cursor-inner {
    margin-left: -3px;
    margin-top: -3px;
    width: 6px;
    height: 6px;
    z-index: 100;
    -webkit-transition: width .3s ease-in-out, height .3s ease-in-out, margin .3s ease-in-out, opacity .3s ease-in-out;
    transition: width .3s ease-in-out, height .3s ease-in-out, margin .3s ease-in-out, opacity .3s ease-in-out;
    background-color: #f75023;
}


.cursor-inner.cursor-hover{
    margin-left: -40px;
    margin-top: -40px;
    width: 80px;
    height: 80px;
    background-color: #f75023;
    opacity: .3
}




.cursor-outer.cursor-hover {
    opacity: 0
}




</style>