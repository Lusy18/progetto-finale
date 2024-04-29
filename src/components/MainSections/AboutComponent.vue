<template>
    <section class="dizme" id="process">
        <div class="dizme_process">
            <div class="container text-center">
                <div class="list">
                    <ul>
                        <li class="animation">
                            <div class="animate__animated animate__fadeInUp" :style="{ animationDuration: '1s' }">
                            <div class="list_inner">
                                <div class="icon">
                                    <span>
                                        <img class="brush"
                                            src="https://marketifythemes.net/html/dizme/img/brushes/process/dark/1.png"
                                            alt />
                                        <img class="svg"
                                            src="https://marketifythemes.net/html/dizme/img/svg/process/target-2.svg"
                                            alt />
                                    </span>
                                </div>
                                <div class="title">
                                    <h3>Pixel Perfect</h3>
                                </div>
                                <div class="text">
                                    <p>Most common methods for designing websites that work well on desktop is
                                        responsive and adaptive design.</p>
                                </div>
                            </div>
                        </div> 
                        </li>
                        <li class="animation">
                            <div class="animate__animated animate__fadeInUp" :style="{ animationDuration: '1s' }">
                            <div class="list_inner">
                                <div class="icon">
                                    <span>
                                        <img class="brush"
                                            src="https://marketifythemes.net/html/dizme/img/brushes/process/dark/2.png"
                                            alt />
                                        <img class="svg"
                                            src="https://marketifythemes.net/html/dizme/img/svg/process/brush-2.svg"
                                            alt />
                                    </span>
                                </div>
                                <div class="title">
                                    <h3>High Quality</h3>
                                </div>
                                <div class="text">
                                    <p>Most common methods for designing websites that work well on desktop is
                                        responsive and adaptive design.</p>
                                </div>
                            </div>
                        </div>
                        </li>
                        <li class="animation">
                           <div class="animate__animated animate__fadeInUp" :style="{ animationDuration: '1s' }">
                            <div class="list_inner">
                                <div class="icon">
                                    <span>
                                        <img class="brush"
                                            src="https://marketifythemes.net/html/dizme/img/brushes/process/dark/3.png"
                                            alt />
                                        <img class="svg"
                                            src="https://marketifythemes.net/html/dizme/img/svg/process/energy-2.svg"
                                            alt />
                                    </span>
                                </div>
                                <div class="title">
                                    <h3>Awesome Idea</h3>
                                </div>
                                <div class="text">
                                    <p>Most common methods for designing websites that work well on desktop is
                                        responsive and adaptive design</p>
                                </div>
                            </div>
                        </div> 
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>
    <section class="dizme" id="about">
        <div class="dizme_about">
            <div class="container">
                <div class="wrapper">
                    <div class="left">
                        <div class="image">
                            <img src="https://marketifythemes.net/html/dizme/img/about/2.jpg"  alt />
                            <div class="numbers year">
                                <div class="wrapper">
                                    <h3><span class="counter" data-from ="0" data-to="18"
                                            data-speed="2000">{{ primoNumero }} </span></h3>
                                    <span class="name">Years of<br />Success</span>
                                </div>
                            </div>
                            <div class="numbers project">
                                <div class="wrapper">
                                    <h3 class="yellowText"><span class="counter" data-from="0"
                                            data-to="9" data-speed="2000">{{ secondoNumero }} </span>K</h3>
                                    <span class="name">Total<br />Projects</span>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="right">
                        <div class="title">
                        <div class="animate__animated animate__fadeInUp" :style="{ animationDuration: '1s' }">   
                            <span>I'm a Designer</span>
                            <h3>I Can Design Anything You Want</h3>
                        </div>  
                        </div>
                        <div class="text">
                        <div class="animate__animated animate__fadeInUp" :style="{ animationDuration: '1s' }">    
                            <p>Hello there! I'm a web designer, and I'm very passionate and dedicated to my work.
                                With 20 years experience as a professional web developer, I have acquired the skills
                                and knowledge necessary to make your project a success. I enjoy every step of the
                                design process, from discussion and collaboration.</p>
                        </div>     
                        </div>
                        <div class="orange_button">
                        <div class="animate__animated animate__fadeInUp" :style="{ animationDuration: '1s' }">  
                            <a class="anchor" href="#contact"><span>Hire Me</span></a>
                        </div>  
                        </div>
                    </div>
                </div>
            </div>
            <div class="brush_1 animate__animated animate__fadeInLeft"><img src="https://marketifythemes.net/html/dizme/img/brushes/about/1.png" alt />
            </div>
            <div class="brush_2 animate__animated animate__fadeInRight"><img src="https://marketifythemes.net/html/dizme/img/brushes/about/2.png" alt />
            </div>
        </div>
    </section>
</template>


<script>


export default {
    name: "AboutComponent",

   
  
    data() {
    return {
      primoNumero: 0,
      secondoNumero: 0,
      contatoreAvviato: false,
    };
 },
 mounted() {
    window.addEventListener('scroll', this.controllaScroll);
 },
 beforeUnmount() {
    window.removeEventListener('scroll', this.controllaScroll);
 },
 methods: {
    controllaScroll() {
      if (!this.contatoreAvviato && window.scrollY >= 400) { // Sostituisci 200 con il punto dello scroll desiderato
        this.avviaContatore();
        this.contatoreAvviato = true; 
      }
    },
    avviaContatore() {
      const incrementoPrimo = setInterval(() => {
        if (this.primoNumero < 18) {
          this.primoNumero++;
        } else {
          clearInterval(incrementoPrimo);
        }
      }, 200); // tempo in millisecondi 0.0005s

      const incrementoSecondo = setInterval(() => {
        if (this.secondoNumero < 9) {
          this.secondoNumero++;
        } else {
          clearInterval(incrementoSecondo);
        }
      }, 200);
    },

 },
}








</script>


<style scoped>

.dizme_process ul li .list_inner {
    width: 100%;
    height: 100%;
    position: relative;

}


.dizme_process .list {
    width: 100%;
    height: auto;

}

.dizme_process {
    width: 100%;
    height: auto;

}

.dizme_section {
    width: 100%;
    height: auto;
    display: flex;

}


.dizme_process ul {
    margin: 0 0 0 -70px;
    list-style-type: none;
}

.dizme_process ul li {
    margin: 0 0 70px;
    width: 33.3333%;
    display: inline-flex;
    padding-left: 70px;
    text-align: center
}


.dizme_process .icon {
    margin-bottom: 30px
}

.dizme_process .icon span {
    position: relative;
    display: inline-block
}

.dizme_process .icon .brush {
    max-width: 100px;
    position: relative
}

.dizme_process .icon .svg {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 60px;
    height: 60px
}

.dizme_process .title {
    margin-bottom: 20px
}

.dizme_process .title h3 {
    font-size: 24px
}


.dizme_about {
    width: 100%;
    height: auto;
    clear: both;
    padding-top: 112px;
    position: relative;
    display: flex;
}

.dizme_about .wrapper {
    width: 100%;
    height: auto;
    display: flex;
    align-items: center;
}

.dizme_about .left {
    width: 50%;
    padding-right: 30px;
}

.dizme_about .left .image {
    position: relative;
}

.dizme_about .left .image img {
    max-height: 500px;
}

.dizme_about .numbers {
    position: absolute;
}

.dizme_about .numbers.year {
    top: 120px;
    left: -80px;
}

.dizme_about .numbers.project {
    bottom: 70px;
    right: -30px;
}

.dizme_about .numbers .wrapper {
    display: flex;
    align-items: center;
    background-color: #4b4f5c;
    border-radius: 8px;
    padding: 24px 40px 31px 36px;
}

.dizme_about .numbers.project .wrapper {
    padding: 14px 30px 11px 26px;
}

.dizme_about .numbers .wrapper h3 {
    font-size: 60px;
    color: #1cbe59;
}

.dizme_about .numbers.project h3 {
    color: #6e50f0;
}

.dizme_about .numbers .wrapper .name {
    font-size: 18px;
    color: white;
    font-weight: 500;
    font-family: 'jost', sans-serif;
    line-height: 1.3;
    padding-left: 17px;
}

.dizme_about .right {
    width: 50%;
    padding-left: 60px;
}

.dizme_about .right .title {
    margin-bottom: 25px;
}

.dizme_about .right .title span {
    display: inline-block;
    color: #f75023;
    font-size: 24px;
    font-weight: 500;
    font-family: jost, sans-serif;
    margin-bottom: 6px;
}

.dizme_about .right .title h3 {
    font-size: 48px;
    max-width: 90%;
    line-height: 1.25;
}

.dizme_about .right .text {
    margin-bottom: 47px
}

.dizme_about .brush_1 {
    position: absolute;
    top: 20px;
    left: 120px
}

.dizme_about .brush_2 {
    position: absolute;
    bottom: -50px;
    right: 0;
}

.orange_button {
    width: 100%;
    height: auto;
}

.orange_button a {
    text-decoration: none;
    color: #fff;
    display: inline-block;
    font-family: "jost", sans-serif;
    font-weight: 500;
    border-radius: 50px;
    border: 2px solid #f75023;
    padding: 14px 48px 13px;
    position: relative;
    overflow: hidden
}

.orange_button span {
    position: relative;
    z-index: 2;
    -webkit-transition: all .3s ease;
    -moz-transition: all .3s ease;
    -ms-transition: all .3s ease;
    -o-transition: all .3s ease;
    transition: all .3s ease
}

.orange_button a:before {
    position: absolute;
    content: "";
    z-index: 0;
    background-color: #f75023;
    left: -5px;
    right: -5px;
    bottom: -5px;
    height: 110%;
    -webkit-transition: all .3s ease;
    -moz-transition: all .3s ease;
    -ms-transition: all .3s ease;
    -o-transition: all .3s ease;
    transition: all .3s ease
}

.orange_button a:hover:before {
    height: 0
}

.orange_button a:hover span {
    color: white
}

.text p {
    color: #706f7c;
    font-family: 'Jost', sans-serif;
    font-size: 18px;
    font-weight: 500;

}













</style>