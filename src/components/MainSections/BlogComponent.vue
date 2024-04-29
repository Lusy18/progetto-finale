<template>
    <div class="section" id="blog">
        <div class="news">
            <div class="container">
                <div class="title" data-align="center">
                    <span>From My Blog</span>
                    <h3>Our Recent Updates, Blog, Tips, <br> Tricks &amp; More</h3>
                </div>
                <div class="news_list">
                    <ul>
                        <li class="up">
                            <div class="list_inner">
                                <div class="image">
                                    <img @click="showModaluno"
                                        src="https://marketifythemes.net/html/dizme/img/news/1.jpg" alt />
                                    <div class="date">
                                        <h3>23</h3>
                                        <span>Dec</span>
                                    </div>
                                    <a class="link" href="#"></a>
                                </div>
                                <div class="details">
                                    <span class="category "><a href="#">Web Development</a></span>
                                    <h3 class="title "><a href="#">Jim Morisson Says when the musics over turn off
                                            the light</a></h3>
                                </div>



                                <!--Inizio modale-->




                                <div class="modal-backdrop" v-show="isModalunoVisible">

                                    <div class="modal  py-5">

                                        <a class="m-x" @click="closeModaluno">x</a>
                                        <img src="https://marketifythemes.net/html/dizme/img/news/1.jpg" alt="">

                                        <div class="modal-body">


                                            <div class="details-modal px-3">

                                                <h3 class="title-modal"><a href="#">Jim Morisson Says when the musics
                                                        over turn off
                                                        the light</a></h3>
                                                <span class="category-modal py-5"><a href="#">Web Development</a></span>
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




                                <!--Fine modale-->

                            </div>
                        </li>




                        <li class="up">
                            <div class="list_inner">
                                <div class="image " style="width:90%;">
                                    <img @click="showModaldue"
                                        src="https://marketifythemes.net/html/dizme/img/news/2.jpg" alt />
                                    <div class="date">
                                        <h3>23</h3>
                                        <span>Dec</span>
                                    </div>
                                    <a class="link" href="#"></a>
                                </div>
                                <div class="details">
                                    <span class="category"><a href="#">Branding</a></span>
                                    <h3 class="title"><a href="#">How to be appreciated for your hard work as a
                                            developer</a></h3>
                                </div>

                            </div>
                            <div class="modal-backdrop" v-show="isModaldueVisible">

                                <div class="modal  py-5">

                                    <a class="m-x" @click="closeModaldue">x</a>
                                    <img src="https://marketifythemes.net/html/dizme/img/news/2.jpg" alt="">

                                    <div class="modal-body">


                                        <div class="details-modal px-3">

                                            <h3 class="title-modal"><a href="#">How to be appreciated for your hard work
                                                    as a
                                                    developer
                                                    the light</a></h3>
                                            <span class="category-modal py-5"><a href="#">Branding</a></span>
                                        </div>
                                        <div class="news_details-modal px-3 pt-3">

                                            <div class="text-modal text start">
                                                <p>Dizme is a leading web design agency with an award-winning design
                                                    team that creates innovative, effective websites that capture your
                                                    brand, improve your conversion rates, and maximize your revenue to
                                                    help grow your business and achieve your goals.</p>
                                                <p>In today’s digital world, your website is the first interaction
                                                    consumers have with your business. That's why almost 95 percent of a
                                                    user’s first impression relates to web design. It’s also why web
                                                    design services can have an immense impact on your company’s bottom
                                                    line.</p>
                                                <p>That’s why more companies are not only reevaluating their website’s
                                                    design but also partnering with Kura, the web design agency that’s
                                                    driven more than $2.4 billion in revenue for its clients. With over
                                                    50 web design awards under our belt, we're confident we can design a
                                                    custom website that drives sales for your unique business.</p>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <div class="modal-footer"></div>
                            </div>
                        </li>
                        <li class="up">
                            <div class="list_inner">
                                <div class="image">
                                    <img @click="showModaltre"
                                        src="https://marketifythemes.net/html/dizme/img/news/3.jpg" alt />

                                    <div class="date">
                                        <h3>23</h3>
                                        <span>Dec</span>
                                    </div>
                                    <a class="link" href="#"></a>
                                </div>
                                <div class="details">
                                    <span class="category"><a href="#">Social Media</a></span>
                                    <h3 class="title"><a href="#">How designers and developers can collaborate
                                            better</a></h3>
                                </div>
                                <div class="modal-backdrop" v-show="isModaltreVisible">

                                    <div class="modal  py-5">

                                        <a class="m-x" @click="closeModaltre">x</a>
                                        <img src="https://marketifythemes.net/html/dizme/img/news/3.jpg" alt="">

                                        <div class="modal-body">


                                            <div class="details-modal px-3">

                                                <h3 class="title-modal"><a href="#">How designers and developers can
                                                        collaborate
                                                        better</a></h3>
                                                <span class="category-modal py-5"><a href="#">Social Media</a></span>
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
            <div class="brush_1"><img src="https://marketifythemes.net/html/dizme/img/brushes/news/1.png" alt /></div>
            <div class="brush_2"><img src="https://marketifythemes.net/html/dizme/img/brushes/news/2.png" alt /></div>
        </div>
    </div>

</template>






<script>


export default {
    name: "BlogComponent",

    data() {
        return {
            isModalunoVisible: false,
            isModaldueVisible: false,
            isModaltreVisible: false,
        };
    },
    methods: {
        showModaluno() {
            this.isModalunoVisible = true;
            this.isModaldueVisible = false;
            this.isModaltreVisible = false;
        },

        showModaldue() {
            this.isModaldueVisible = true;
            this.isModalunoVisible = false;
            this.isModaltreVisible = false;
        },
        showModaltre() {
            this.isModaltreVisible = true;
            this.isModalunoVisible = false;
            this.isModaldueVisible = false;
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
    }

}

</script>





<style scoped>
.title span {
    font-size: 24px;
    font-weight: 500;
    color: #f75023;
    font-family: 'jost', sans-serif;
    display: inline-block;
    margin-bottom: 6px;
}

.title h3 {
    font-size: 40px;
    line-height: 1.25;
    margin-bottom: 23px
}


.title {
    width: 100%;
    max-width: 680px;
    height: auto;
    clear: both;
    text-align: center;
    margin: 0 auto
}


.news {
    width: 100%;
    height: auto;
    clear: both;
    display: left;
    padding-top: 50px;
    margin-bottom: 100px;
    position: relative
}

.news .news_list {
    width: 100%;
    height: auto;
    clear: both;
    display: inline-flex;
    padding-top: 65px
}

.news ul .main {
    margin: 0 0 0 0px;
    list-style-type: none
}

.news ul li {
    margin: 0 0 25px;
    width: 33.3333%;
    display: inline-flex;
    padding-left: 25px
}

.news ul li .list_inner {
    width: 100%;
    height: 100%;
    clear: both;
    display: inline;
    position: relative
}

.up {
    width: 1160px;
    margin: 0 auto;
}

.list_inner {
    width: 40%;
}

.image {
    width: 100%;
    height: 100%;
    position: relative;
    overflow: hidden;
    border-radius: 12px;



}

.image img {
    display: block;
    transform: scale(1);
    transition: all .2s linear;
}

.image img:hover {
    transform: scale(1.1);
}


img {
    max-width: 100%;
}


.news ul li .date {
    position: absolute;
    top: 18px;
    right: 18px;
    z-index: 2;
    display: inline-block;
    background-color: #1cbe59;
    text-align: center;
    border-radius: 12px;
    padding: 10px 19px 7px;
    line-height: 1
}

.news ul li .date h3 {
    font-size: 24px;
    color: #fff;
    font-family: inherit;
    line-height: 1.2
}


.news ul li .details .category a {
    font-size: 16px;
    color: #f75023;
    font-family: 'jost', 'sans-serif';
    text-decoration: none;
    font-weight: 500;
    display: inline-block;
    margin-bottom: 2px
}

.news ul li .details .title {
    line-height: 1.4
}

.news ul li .details .title a {
    font-size: 21px;
    color: white;
    display: inline-block;
    text-decoration: none;
    text-align: left;
    -webkit-transition: all .3s ease;
    -moz-transition: all .3s ease;
    -ms-transition: all .3s ease;
    -o-transition: all .3s ease;
    transition: all .3s ease
}

.news ul li .details .title a:hover {
    color: #f75023
}

.news .news_hidden {
    display: none;
    opacity: 0;
    visibility: hidden;
    position: absolute;
    z-index: -11
}


.news .brush_1 {
    position: absolute;
    top: 150px;
    left: 110px
}

.news .brush_2 {
    position: absolute;
    top: -60px;
    right: 0
}



/*modal*/
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
    color: #a7a3b5;

}
</style>