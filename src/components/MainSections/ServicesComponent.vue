<template>
    <section class="section" id="service">
        <div class="services">
            <div class="container">
                <div class="title data-align center">
                    <span>Services</span>
                    <h3>What I Do for Clients</h3>
                    <p>Most common methods for designing websites that work well on desktop is responsive and
                        adaptive design</p>
                </div>
                <div class="service_list">
                    <ul>
                        <li class="left">
                            <div class="list_inner" @mousemove="onMouseMove" @mouseleave="reset">
                                <span class="icon" @click="showModaluno">
                                    <img class="svg"
                                        src="https://marketifythemes.net/html/dizme/img/svg/service/anchor.svg" alt />
                                    <img class="back"
                                        src="https://marketifythemes.net/html/dizme/img/brushes/service/dark/1.png"
                                        alt />
                                </span>
                                <div class="title">
                                    <h3>Creative Design</h3>
                                    <span class="price">Starts from <span class="numberText">$99</span></span>
                                </div>
                                <div class="text">
                                    <p>Web design refers to the design of websites that are displayed on the
                                        internet. It usually refers to the user experience aspects of website
                                        development</p>
                                </div>
                                <a class="link" href="#"></a>


                                <!--Inizio modale-->


                        <div class="modal-backdrop" v-show="isModalunoVisible">

                            <div class="modal  py-5 my-5">

                                <a class="m-x" @click="closeModaluno">x</a>
                                    <img src="https://marketifythemes.net/html/dizme/img/service/1.jpg" alt="">

                                        <div class="modal-body">


                                            <div class="details-modal px-3">

                                                <h3 class="title-modal"><a href="#">Creative Design</a></h3>
                                                <span class="category-modal py-5">Starts from<a href="#"> $99</a></span>
                                            </div>
                                            <div class="news_details-modal px-3 pt-3">

                                                <div class="text-modal text start">
                                                    <p>Dizme is a leading web design agency with an award-winning design
                                                        team that creates innovative, effective websites that capture
                                                        your
                                                        brand, improve your conversion rates, and maximize your revenue
                                                        to
                                                        help grow your business and achieve your goals.</p>
                                                    <p>In today’s digital world, your website is the first interaction
                                                        consumers have with your business. That's why almost 95 percent
                                                        of a
                                                        user’s first impression relates to web design. It’s also why web
                                                        design services can have an immense impact on your company’s
                                                        bottom
                                                        line.</p>
                                                    <p>That’s why more companies are not only reevaluating their
                                                        website’s
                                                        design but also partnering with Kura, the web design agency
                                                        that’s
                                                        driven more than $2.4 billion in revenue for its clients. With
                                                        over
                                                        50 web design awards under our belt, we're confident we can
                                                        design a
                                                        custom website that drives sales for your unique business.</p>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="modal-footer">
                                    </div>
                                    </div>


                                <!--Fine modale-->

                            </div>
                        </li>
                        <li class="right">
                            <div class="list_inner">
                                <span class="icon" @click="showModaldue" >
                                    <img class="svg"
                                        src="https://marketifythemes.net/html/dizme/img/svg/service/physics.svg" alt />
                                    <img class="back"
                                        src="https://marketifythemes.net/html/dizme/img/brushes/service/dark/2.png"
                                        alt />
                                </span>
                                <div class="title">
                                    <h3>Graphic Design</h3>
                                    <span class="price">Starts from <span class="numberText">$199</span></span>
                                </div>
                                <div class="text">
                                    <p>Web design refers to the design of websites that are displayed on the
                                        internet. It usually refers to the user experience aspects of website
                                        development</p>
                                </div>
                                <a class="link" href="#"></a>
                                <div class="modal-backdrop" v-show="isModaldueVisible">

                                    <div class="modal  py-5">

                                        <a class="m-x" @click="closeModaldue">x</a>
                                        <img src="https://marketifythemes.net/html/dizme/img/service/2.jpg" alt="">

                                        <div class="modal-body">


                                            <div class="details-modal px-3">

                                                <h3 class="title-modal"><a href="#">Graphic Design</a></h3>
                                                <span class="category-modal py-5">Starts from<a href="#">
                                                        $199</a></span>
                                            </div>
                                            <div class="news_details-modal px-3 pt-3">

                                                <div class="text-modal text start">
                                                    <p>Dizme is a leading web design agency with an award-winning design
                                                        team that creates innovative, effective websites that capture
                                                        your
                                                        brand, improve your conversion rates, and maximize your revenue
                                                        to
                                                        help grow your business and achieve your goals.</p>
                                                    <p>In today’s digital world, your website is the first interaction
                                                        consumers have with your business. That's why almost 95 percent
                                                        of a
                                                        user’s first impression relates to web design. It’s also why web
                                                        design services can have an immense impact on your company’s
                                                        bottom
                                                        line.</p>
                                                    <p>That’s why more companies are not only reevaluating their
                                                        website’s
                                                        design but also partnering with Kura, the web design agency
                                                        that’s
                                                        driven more than $2.4 billion in revenue for its clients. With
                                                        over
                                                        50 web design awards under our belt, we're confident we can
                                                        design a
                                                        custom website that drives sales for your unique business.</p>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="modal-footer"></div>
                                </div>


                            </div>
                        </li>
                        <li class="left">
                            <div class="list_inner">
                                <span class="icon" @click="showModaltre">
                                    <img class="svg"
                                        src="https://marketifythemes.net/html/dizme/img/svg/service/contact.svg" alt />
                                    <img class="back"
                                        src="https://marketifythemes.net/html/dizme/img/brushes/service/dark/3.png"
                                        alt />
                                </span>
                                <div class="title">
                                    <h3>UI/UX Design</h3>
                                    <span class="price">Starts from <span class="numberText">$299</span></span>
                                </div>
                                <div class="text">
                                    <p>Web design refers to the design of websites that are displayed on the
                                        internet. It usually refers to the user experience aspects of website
                                        development</p>
                                </div>
                                <a class="link" href="#"></a>

                                <div class="modal-backdrop" v-show="isModaltreVisible">

                                    <div class="modal  py-5">

                                        <a class="m-x" @click="closeModaltre">x</a>
                                        <img src="https://marketifythemes.net/html/dizme/img/service/3.jpg" alt="">

                                        <div class="modal-body">


                                            <div class="details-modal px-3">

                                                <h3 class="title-modal"><a href="#">UI/UX Design</a></h3>
                                                <span class="category-modal py-5">Starts from<a href="#">
                                                        $299</a></span>
                                            </div>
                                            <div class="news_details-modal px-3 pt-3">

                                                <div class="text-modal text start">
                                                    <p>Dizme is a leading web design agency with an award-winning design
                                                        team that creates innovative, effective websites that capture
                                                        your
                                                        brand, improve your conversion rates, and maximize your revenue
                                                        to
                                                        help grow your business and achieve your goals.</p>
                                                    <p>In today’s digital world, your website is the first interaction
                                                        consumers have with your business. That's why almost 95 percent
                                                        of a
                                                        user’s first impression relates to web design. It’s also why web
                                                        design services can have an immense impact on your company’s
                                                        bottom
                                                        line.</p>
                                                    <p>That’s why more companies are not only reevaluating their
                                                        website’s
                                                        design but also partnering with Kura, the web design agency
                                                        that’s
                                                        driven more than $2.4 billion in revenue for its clients. With
                                                        over
                                                        50 web design awards under our belt, we're confident we can
                                                        design a
                                                        custom website that drives sales for your unique business.</p>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="modal-footer"></div>
                                </div>

                            </div>
                        </li>
                        <li class="right">
                            <div class="list_inner tilt-effect">
                                <span class="icon" @click="showModalquattro">
                                    <img class="svg"
                                        src="https://marketifythemes.net/html/dizme/img/svg/service/web.svg" alt />
                                    <img class="back"
                                        src="https://marketifythemes.net/html/dizme/img/brushes/service/dark/4.png"
                                        alt />
                                </span>
                                <div class="title">
                                    <h3>Web Design</h3>
                                    <span class="price">Starts from <span class="numberText">$399</span></span>
                                </div>
                                <div class="text">
                                    <p>Web design refers to the design of websites that are displayed on the
                                        internet. It usually refers to the user experience aspects of website
                                        development</p>
                                    <div class="bg"></div>
                                </div>
                                <a class="link" href="#"></a>

                                <div class="modal-backdrop" v-show="isModalquattroVisible">

                                    <div class="modal  py-5">

                                        <a class="m-x" @click="closeModalquattro">x</a>
                                        <img src="https://marketifythemes.net/html/dizme/img/service/4.jpg" alt="">

                                        <div class="modal-body">


                                            <div class="details-modal px-3">

                                                <h3 class="title-modal"><a href="#">Web Design</a></h3>
                                                <span class="category-modal py-5">Starts from<a href="#">
                                                        $399</a></span>
                                            </div>
                                            <div class="news_details-modal px-3 pt-3">

                                                <div class="text-modal text start">
                                                    <p>Dizme is a leading web design agency with an award-winning design
                                                        team that creates innovative, effective websites that capture
                                                        your
                                                        brand, improve your conversion rates, and maximize your revenue
                                                        to
                                                        help grow your business and achieve your goals.</p>
                                                    <p>In today’s digital world, your website is the first interaction
                                                        consumers have with your business. That's why almost 95 percent
                                                        of a
                                                        user’s first impression relates to web design. It’s also why web
                                                        design services can have an immense impact on your company’s
                                                        bottom
                                                        line.</p>
                                                    <p>That’s why more companies are not only reevaluating their
                                                        website’s
                                                        design but also partnering with Kura, the web design agency
                                                        that’s
                                                        driven more than $2.4 billion in revenue for its clients. With
                                                        over
                                                        50 web design awards under our belt, we're confident we can
                                                        design a
                                                        custom website that drives sales for your unique business.</p>
                                                </div>
                                            </div>
                                        </div>


                                    </div>
                                    <div class="modal-footer"></div>
                                </div>


                            </div>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="brush_1"><img src="https://marketifythemes.net/html/dizme/img/brushes/service/5.png" alt />
            </div>
            <div class="brush_2"><img src="https://marketifythemes.net/html/dizme/img/brushes/service/6.png" alt />
            </div>
        </div>

    </section>
</template>


<script>


export default {
    name: "ServicesComponent",

    

    // mounted() {
    //     this.tiltEffect = tilt('service_list', {
    //         maxTilt: 15,
    //         perspective: 1400,
    //         easing: "cubic-bezier(.03,.98,.52,.99)",
    //         speed: 1200,
    //         glare: true,
    //         maxGlare: 0.2,
    //         scale: 1.04
    //     });
    // },
    // beforeDestroy() {
    //     if (this.tiltEffect) {
    //         this.tiltEffect.destroy();
    //     }
    // }

    data() {
        return {
            isModalunoVisible: false,
            isModaldueVisible: false,
            isModaltreVisible: false,
            isModalquattroVisible: false,
        };
    },
    methods: {
        showModaluno() {
            this.isModalunoVisible = true;
            this.isModaldueVisible = false;
            this.isModaltreVisible = false;
            this.isModalquattroVisible = false;

        },

        showModaldue() {
            this.isModaldueVisible = true;
            this.isModalunoVisible = false;
            this.isModaltreVisible = false;
            this.isModalquattroVisible = false;
        },
        showModaltre() {
            this.isModaltreVisible = true;
            this.isModalunoVisible = false;
            this.isModaldueVisible = false;
            this.isModalquattroVisible = false;
        },
        showModalquattro() {
            this.isModalquattroVisible = true;
            this.isModalunoVisible = false;
            this.isModaldueVisible = false;
            this.isModaltreVisible = false;
        },


        closeModaluno() {
            this.isModalunoVisible = false;
        },

        closeModaldue() {
            this.isModaldueVisible = false;
        },
        closeModaltre() {
            this.isModaltreVisible = false;
        },
        closeModalquattro() {
            this.isModalquattroVisible = false;
        },
    }









};



</script>



<style scoped>

.title {
    width: 100%;
    max-width: 680px;
    height: auto;
    clear: both;
    text-align: center;
    margin: 0 auto
}

.title h3 {
    font-size: 48px;
    line-height: 1.25;
    margin-bottom: 23px
}

.title p {
    color: #9e9cad;
    
}

.title span {
    font-size: 24px;
    font-weight: 500;
    color: #f75023;
    font-family: 'jost', sans-serif;
    display: inline-block;
    margin-bottom: 6px;
}


.services {
    width: 100%;
    height: auto;
    clear: both;
    display: flex;
    padding-top: 178px;
    margin-bottom: 160px;
    position: relative
}

.services .service_list {
    width: 100%;
    height: auto;
    clear: both;
    display: flex;
    padding-top: 86px
}

.services .service_list ul {
    margin: 0 0 0 -25px;
    list-style-type: none;
    display: flex;
    flex-wrap: wrap;
    position: relative;
    z-index: 3
}

.services .service_list ul li {
    margin: 0 0 25px;
    width: 50%;
    display: flex;
    padding-left: 25px
}

.services .service_list ul li .list_inner {
    width: 100%;
    height: 100%;
    display: left;
    position: relative;
    border-radius: 12px;
    background-color: #4b4f5c;
    box-shadow: 18px 0 87px rgba(10, 15, 70, .07);
    padding: 65px 65px 65px 195px;


}



.services .service_list .title h3 {
    font-size: 30px;
    margin-bottom: 16px;
    position: relative;
    z-index: 2;
    
}

.services .service_list .price {
    font-weight: 500;
    font-size: 21px;
    color: white;
    font-family: 'jost', sans-serif;
    
}

.services .service_list .price span {
    font-size: 24px;
    color: #f75023
}

.services .service_list .icon {
    position: absolute;
    left: 65px;
    top: 65px;
    width: 95px;
    height: 95px
}

.services .service_list .icon .svg {
    height: 40px;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    position: absolute;
    z-index: 2;

}

.services .service_list .icon .back {
    position: absolute;
    max-width: 95px;
    top: 0
}


.services .image {
    opacity: 0;
    visibility: hidden;
    display: none;
    position: absolute;
    z-index: -111
}

.services .service_hidden_details {
    opacity: 0;
    visibility: hidden;
    display: none;
    position: absolute;
    z-index: -111
}


.services .brush_1 {
    position: absolute;
    top: 300px;
    left: 0
}

.services .brush_1 img {
    max-width: 460px
}

.services .brush_2 {
    position: absolute;
    top: 0;
    right: 0
}

.icon {
    cursor: pointer;
}

/*modal*/

.modal{
    z-index: 1050;
}

.modal-header {
    border-bottom: none;
}

.modal-dialog {
    max-width: 90%;
}


.m-x {
    font-size: 30px;
    color: white;
    margin-bottom: 20px;
    text-decoration: none;
    cursor: pointer;
    transform: translateX(700px);
}

.modal-backdrop {
    position: fixed;
    background-color: #020202d7;
    display: flex;
    justify-content: center;
    align-items: center;
    padding-top: 50px;
    padding-bottom: 20px;
    overflow-y: auto;
    overscroll-behavior: contain;
    /* Previene lo scorrimento della pagina principale */
    z-index: 20999 !important;


}


.modal {
    background: #34353a;
    display: flex;
    flex-direction: column;
    width: 800px;
    margin: 40px;
    position: relative;
    overflow-y: auto;
    /*fa scrollare lo stesso la modale*/

}


.modal-footer {
    padding-top: 45px;
    display: flex;
    justify-content: center;
    flex-direction: column;
    border-top: none;
}



.modal-body {
    border-top: none;
    border-bottom: none;
    font-family: "Roboto", sans-serif;
    position: relative;

}



.modal img {
    width: 712px;
    border-radius: 20px;
    text-align: center;
    justify-content: center;
    align-items: center;
    display: flex;
    margin-left: 30px;
}

.text-modal {
    color: #a7a3b5;
    text-align: left;
    left: 0;
    padding-left: -20px;
}


.title-modal a {
    text-decoration: none;
    color: white;
}

.category-modal a {
    text-decoration: none;
    color: #f75023;

}

.category-modal {
    color: white;
}
</style>