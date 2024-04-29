<template>
    <div class="section" id="jumbo">
        <div class="smith">
            <div class="background" data-img-url="img/slider/2.jpg"></div>
            <div class="container">
                <div class="content">
                    <div class="details">
                        <div class="hello">
                            <h3 class="orangeText">Hello, I'm</h3>
                        </div>
                        <div class="name">
                            <h3>James Smith</h3>
                        </div>
                        <div class="job">
                            <p>A <span class="greenText">Creative Designer</span> From <span class="yellowText">New
                                    York</span></p>
                        </div>
                        <div class="text">
                            <p>I'm creative designer based in New York, and I'm very passionate and 
                                dedicated to my work.</p>
                        </div>
                        <div class="button">
                            <div class="orange_button">
                                <a class="anchor" href="#about"><span>About Me</span></a>
                            </div>
                            <div class="social">
                                <ul>
                                    <li><a href="#"><i class="fab fa-facebook-f"></i></a></li>
                                    <li><a href="#"><i class="fab fa-twitter"></i></a></li>
                                    <li><a href="#"><i class="fab fa-linkedin-in"></i></a></li>
                                    <li><a href="#"><i class="fab fa-behance"></i></a></li>
                                </ul>
                            </div>
                        </div>
                    </div>
                    <div class="man">
                        <div class="image">
                            <img src="https://marketifythemes.net/html/dizme/img/slider/avatar.png" alt />
                            <span class="logo illustrator anim_moveBottom"><img class="svg"
                                    src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/fb/Adobe_Illustrator_CC_icon.svg/512px-Adobe_Illustrator_CC_icon.svg.png"
                                    alt /></span>
                            <span class="logo photoshop anim_moveBottom"><img class="svg"
                                    src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/af/Adobe_Photoshop_CC_icon.svg/1051px-Adobe_Photoshop_CC_icon.svg.png"
                                    alt /></span>
                            <span class="logo figma anim_moveBottom"><img class="svg"
                                    src="https://www.svgrepo.com/show/452202/figma.svg" alt /></span>
                        </div>
                    </div>
                </div>
            </div>
            <div class="down">
                <a class="anchor" href="#process">
                    <svg width="26px" height="100%" viewBox="0 0 247 390" version="1.1"
                        xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"
                        style="fill-rule:evenodd;clip-rule:evenodd;stroke-linecap:round;stroke-linejoin:round;stroke-miterlimit:1.5;">
                        <path id="wheel" d="M123.359,79.775l0,72.843"
                            style="fill:none;stroke:#fff;stroke-width:20px;" />
                        <path id="mouse"
                            d="M236.717,123.359c0,-62.565 -50.794,-113.359 -113.358,-113.359c-62.565,0 -113.359,50.794 -113.359,113.359l0,143.237c0,62.565 50.794,113.359 113.359,113.359c62.564,0 113.358,-50.794 113.358,-113.359l0,-143.237Z"
                            style="fill:none;stroke:#fff;stroke-width:20px;" />
                    </svg>
                </a>
            </div>
        </div>
    </div>
</template>


<script>


export default {
    name: "JumboComponent",
}

</script>

<style scoped>



.smith {
    width: 100%;
    height: 100vh;
    display: flex;
    position: relative;
    margin-bottom: 25%;
}


.smith .content {
    width: 100%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between
}

.smith .details {
    width: 50%;
    padding-right: 20px
}

.smith .hello h3 {
    font-size: 25px;
    font-weight: bold;
}

.smith .name {
    margin-bottom: 18px;
}

.smith .name h3 {
    font-size: 60px
}

.smith .job {
    margin-bottom: 35px
}

.smith .job p {
    font-size: 18px;
    color: white;
    font-weight: 600;
}

.smith .text {
    margin-bottom: 21px;


}

.smith .text p {
    font-size: 18px;
    line-height: 1.5
}

.smith .button {
    display: flex;
    align-items: center
}

.smith .orange_button {
    width: auto
}

.orange_button {
    width: 100%;
    height: auto;
}

.orange_button a {
    text-decoration: none;
    color: #fff;
    display: inline-block;
    font-family: 'jost', sans-serif;
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
    color: white;
}

.smith .social {
    padding-left: 27px;
    position: relative;
    top: -4px;
    padding: 15px;

}

.smith .social ul {
    margin: 0;
    list-style-type: none;
}


.smith .social ul li {
    margin: 0 5px 0 0;
    display: inline-block;
}

.smith .social ul li:last-child {
    margin-right: 0;
}

.smith .social ul li a {
    text-decoration: none;
    color: white;
    padding-inline: 5px;
}

.smith .image {
    position: relative;
}

.smith .man {
    width: 50%;
    padding-left: 100px;
}

.smith .man img {
    max-height: 390px;
}

.smith .logo {
    display: inline-block;
    width: 40px;
    height: 40px;
    border-radius: 8px;
    position: absolute;
    box-shadow: 24px 0 72px rgba(54, 32, 152, .3)
}

.smith .logo.illustrator {
    background-color: #390000;
    top: 20px;
    left: -30px;
}

.smith .logo.photoshop {
    background-color: #001631;
    right: 70px;
    top: 80px;
}

.smith .logo.figma {
    background-color: #fff;
    bottom: 30px;
    left: 120px;
}

.smith .logo .svg {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 40px;
    height: 40px
}

.smith .logo.illustrator .svg {
    color: #ff9a00
}

.smith .logo.photoshop .svg {
    color: #00a9ff
}

.down {
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
    bottom: 60px;
    z-index: 5
}

.down svg {
    width: 35px;
    height: 35px
}

.down svg #wheel {
    animation: scroll ease 2s infinite
}

/* movimento immagine mouse piccolina */

@keyframes scroll {         
    0% {
        transform: translateY(0)
    }

    30% {
        transform: translateY(60px)
    }
}

.animPulse {
    animation: animPulse 3s linear 0s infinite alternate
}

@keyframes animPulse {
    0% {
        transform: scale(1)
    }

    100% {
        transform: scale(1.2)
    }
}

.anim_moveLeft {
    animation: animMoveLeft 3s linear 0s infinite alternate
}

@keyframes animMoveLeft {
    0% {
        transform: translateX(0px)
    }

    100% {
        transform: translateX(-20px)
    }
}

.anim_moveRight {
    animation: anim_moveRight 3s linear 0s infinite alternate
}

@keyframes anim_moveRight {
    0% {
        transform: translateX(0px)
    }

    100% {
        transform: translateX(20px)
    }
}

.anim_moveTop {
    animation: anim_moveTop 3s linear 0s infinite alternate
}

@keyframes anim_moveTop {
    0% {
        transform: translateY(0px)
    }

    100% {
        transform: translateY(-20px)
    }
}

.anim_moveBottom {
    animation: anim_moveBottom 3s linear 0s infinite alternate
}

@keyframes anim_moveBottom {
    0% {
        transform: translateY(0px)
    }

    100% {
        transform: translateY(20px)
    }
}

.svg {
    fill: currentcolor;
    width: 15px;
    height: 15px
}

.orangeText{
    color: #f75023;;

}

.greenText{
    color: #1cbe59;
}

.yellowText{
    color:#e8be5b
}




</style>