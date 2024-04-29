<template>
 <div class="news_section">
            <div class="news_subscribe">
                <div class="container">
                    <div class="inner">
                        <div class="background">
                            <div class="dots" data-img-url="https://marketifythemes.net/html/dizme/img/subscribe/dots.jpg" style='background-image: url("https://marketifythemes.net/html/dizme/img/subscribe/dots.jpg");'></div>
                            <div class="overlay"></div>
                        </div>
                        <div class="content">
                             <div class="animate__animated animate__fadeInLeft" :style="{ animationDuration: '1s' }">
                                <span class="subtitle">Subscribe Now</span>
                                <h3 class="title">Get My Newsletter</h3>
                                <p class="text">Get latest news, updates, tips and trics in your inbox</p>
                            </div>
                            <div class="animate__animated animate__fadeInRight" :style="{ animationDuration: '1s' }">
                                <div class="field">
                                    <input type="text" placeholder="Your email here">
                                    <input type="submit" value="Send Now" />
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
</template>


<script>


export default {
name: "SubscriveComponent",
}

</script>

<style scoped>

.news_subscribe {
    display: flex;
    width: 100%;
    height: auto;
  
    
}

.news_subscribe .inner {
    width: 100%;
    height: auto;
    position: relative
}

.news_subscribe .background {
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    border-radius: 12px
}

.news_subscribe .background .dots {
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
    border-radius: 12px
}

.news_subscribe .background .overlay {
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    background-color: rgb(128, 103, 240, .92);
    z-index: 1;
    border-radius: 12px
}

.news_subscribe .content {
    position: relative;
    z-index: 2;
    display: flex;
    align-items: center;
    padding: 83px 90px 86px
}

.news_subscribe  .animate__fadeInRight{
    width: 30%;
    padding-right: 15px;
    
}

.news_subscribe .subtitle {
    display: inline-block;
    font-size: 21px;
    font-weight: 500;
    color: #fff;
    font-family: 'jost', sans-serif;
    margin-bottom: 5px
}

.news_subscribe .title {
    color: #fff;
    font-size: 48px;
    margin-bottom: 10px
}

.news_subscribe .text {
    color: #fff
}

.news_subscribe .animate__fadeInLeft{
    width: 50%;
    padding-left: 30px;
}

.news_subscribe .field {
    width: 100%;
    position: relative;
    
}

.news_subscribe .field input[type=text] {
    width: 100%;
    height: 72px;
    /* border-radius: 12px; */
    border-bottom-left-radius: 12px;
    border-top-left-radius: 12px;
    color: #6f6b80;
    /* background-color: #fff; */
    padding-left: 100px
}

.news_subscribe .field input[type=text]:focus {
    outline: none
}

.news_subscribe .field input[type=submit] {
    display:inline-flex;
    position:absolute;
    right: 100;
    top: 0;
    height: 72px;
    border-top-right-radius: 12px;
    border-bottom-right-radius: 12px;
    color: #fff;
    font-family: 'jost', sans-serif;
    font-size: 18px;
    font-weight: 500;
    background-color: #f75023;
    padding: 0 35px 0
}


</style>