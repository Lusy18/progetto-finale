<template>

<div>
    <nav v-if="isMobile" class="mobile-menu">
      <!-- Menu per dispositivi mobili -->
    </nav>
    <nav v-else class="desktop-menu">
      <!-- Menu per desktop -->
    </nav>
 </div>
     
         


    <section>
        <div id="preloader" v-if="isLoading" >
        <div class="loader_line"></div>
        </div>
        <div class="header">
            <div class="container">
                <div class="inner">
                    <div class="logo">
                        <a href="#"><img src="https://marketifythemes.net/html/dizme/img/logo/dark.png" alt /></a>
                    </div>
                    <div class="menu">
                        <ul class="anchor_nav">
                            <li class="current"><a href="#home">Home</a></li>
                            <li><a href="#about">About</a></li>
                            <li><a href="#portfolio">Portfolio</a></li>
                            <li><a href="#service">Service</a></li>
                            <li><a href="#blog">Blog</a></li>
                            <li><a href="#contact">Contact</a></li>
                            <li class="download_cv"><a href="img/cv/1.jpg" download><span>Download CV</span></a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>


<script>

export default {
    name: "HeaderComponent",
    data() {
    return {
      isLoading: false,
    //   responsive
      isMobile: window.innerWidth <= 768
    };
 },
 methods: {
    loadData() {
      this.isLoading = true;
      // Simula il caricamento dei dati
      setTimeout(() => {
        this.isLoading = false;
      }, 2500);
    },
    // responsive
    checkScreenSize() {
      this.isMobile = window.innerWidth <= 768;
    }

 },

 mounted() {
    this.loadData();
    // responsive
    window.addEventListener('resize', this.checkScreenSize);
 },
 beforeUnmount() {
    window.removeEventListener('resize', this.checkScreenSize);
 },



}

</script>




<style scoped>


.header {
    background-color: #3e4454;
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    z-index: 10;
    padding: 25px 0;
    -webkit-transition: all .3s ease;
    -moz-transition: all .3s ease;
    -ms-transition: all .3s ease;
    -o-transition: all .3s ease;
    transition: all .3s ease
}


.header .inner {
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between
}

.header.animate {
    background-color: #fff;
    padding: 20px 0;
    box-shadow: 0 0 10px rgba(0, 0, 0, .1)
}

.header .logo img {
    max-width: 110px;
    max-height: 100px
}

.header .menu ul {
    margin: 0;
    list-style-type: none;
    display: flex;
    align-items: center
}

.header .menu ul li {
    margin: 0 30px 0 0;
    display: inline-block
}

.header .menu ul li:last-child {
    margin-right: 0
}

.header .menu ul li.current a {
    color: #f75023
}

.header .menu ul li a:hover {
    color: #f75023
}

.header .menu ul li a {
    text-decoration: none;
    color: white;
    font-weight: 600;
    font-family: 'Jost', sans-serif;
    -webkit-transition: all .3s ease;
    -moz-transition: all .3s ease;
    -ms-transition: all .3s ease;
    -o-transition: all .3s ease;
    transition: all .3s ease
}

.header .download_cv {
    position: relative;
    top: 3px
}

.header .download_cv a {
    border: 2px solid #f75023;
    border-radius: 50px;
    padding: 8px 33px 7px;
    position: relative;
    overflow: hidden;
    display: inline-block;
}

.header .download_cv span {
    position: relative;
    z-index: 2;
    -webkit-transition: all .3s ease;
    -moz-transition: all .3s ease;
    -ms-transition: all .3s ease;
    -o-transition: all .3s ease;
    transition: all .3s ease
}

.header .download_cv a:before {
    position: absolute;
    content: "";
    z-index: 0;
    background-color: #f75023;
    left: -5px;
    right: -5px;
    bottom: -5px;
    height: 0;
    -webkit-transition: all .3s ease;
    -moz-transition: all .3s ease;
    -ms-transition: all .3s ease;
    -o-transition: all .3s ease;
    transition: all .3s ease
}

.header .download_cv a:hover:before {
    height: 115%
}

.header .download_cv a:hover span {
    color: #fff
}

/* caricamento pagina web con linea verticale effetto show */

#preloader {
    position: fixed;
    left: 0;
    top: 0;
    height: 100vh;
    width: 100%;
    z-index: 99999;
    display: flex
}

#preloader:before,
#preloader:after {
    content: '';
    position: absolute;
    left: 0;
    top: 0;
    width: 50%;
    height: 100%;
    z-index: -1;
    background-color: orangered;
    -webkit-transition: all .3s ease 0s;
    -o-transition: all .3s ease 0s;
    transition: all .3s ease 0s
}

#preloader:after {
    left: auto;
    right: 0
}

#preloader .loader_line {
    margin: auto;
    width: 1px;
    height: 250px;
    position: relative;
    overflow: hidden;
    -webkit-transition: all .8s ease 0s;
    -o-transition: all .8s ease 0s;
    transition: all .8s ease 0s
}

.loader_line:before {
    content: '';
    position: absolute;
    left: 0;
    top: 50%;
    width: 1px;
    height: 0%;
    -webkit-transform: translateY(-50%);
    -ms-transform: translateY(-50%);
    -o-transform: translateY(-50%);
    transform: translateY(-50%);
    background-color: #fff;
    -webkit-animation: lineheight 1000ms ease-in-out 0s forwards;
    -o-animation: lineheight 1000ms ease-in-out 0s forwards;
    animation: lineheight 1000ms ease-in-out 0s forwards
}

.loader_line:after {
    content: '';
    position: absolute;
    left: 0;
    top: 0;
    width: 1px;
    height: 100%;
    background-color: #999;
    -webkit-transform: translateY(-100%);
    -ms-transform: translateY(-100%);
    -o-transform: translateY(-100%);
    transform: translateY(-100%);
    -webkit-animation: lineround 1200ms linear 0s infinite;
    -o-animation: lineround 1200ms linear 0s infinite;
    animation: lineround 1200ms linear 0s infinite;
    animation-delay: 2000ms
}

@keyframes lineheight {
    0% {
        height: 0%
    }

    100% {
        height: 100%
    }
}

@keyframes lineround {
    0% {
        -webkit-transform: translateY(-100%);
        -ms-transform: translateY(-100%);
        -o-transform: translateY(-100%);
        transform: translateY(-100%)
    }

    100% {
        -webkit-transform: translateY(200%);
        -ms-transform: translateY(200%);
        -o-transform: translateY(200%);
        transform: translateY(200%)
    }
}

.preloaded .loader_line:after {
    opacity: 0
}

.preloaded .loader_line {
    opacity: 0;
    height: 100% 
}

.preloaded:before,
.preloaded:after {
    -webkit-animation: preloadedzero 300ms ease-in-out 500ms forwards;
    -o-animation: preloadedzero 300ms ease-in-out 500ms forwards;
    animation: preloadedzero 300ms ease-in-out 500ms forwards
}

@keyframes preloadedzero {
    0% {
        width: 50%
    }

    100% {
        width: 0%
    }
}










</style>
