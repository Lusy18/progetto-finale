<template>

    <section id="portfolio">
        <div class="container">
            <div class="brush_1 animate__animated animate__zoomIn"><img src="https://marketifythemes.net/html/dizme/img/brushes/portfolio/1.png" alt /></div>
            <div class="row align-items-center mt-5 gy-5 gy-lg-0">
                <div class="col text-center">
                    <span>Portfolio</span>
                    <h3>My Amazing Works</h3>
                    <p>Most common methods for designing websites that work well on desktop <br>
                        is responsive and adaptive design
                    </p>
                    <div class="filter">
                        <ul>
                            <li class="current"><a @click="filterImages('all')">All</a></li>
                            <li><a @click="filterImages('youtube')">Youtube</a></li>
                            <li><a @click="filterImages('vimeo')">Vimeo </a></li>
                            <li><a @click="filterImages('soundcloud')">Soundcloud</a></li>
                            <li> <a @click="filterImages('popup')">Popup</a></li>
                            <li><a @click="filterImages('detail')">Detail</a></li>
                        </ul>
                    </div>
                    <div class="gallery">
                        <div class="grid-container">
                            <div v-for="(image, index) in images" :key="index" :class="'image-' + index"
                                class="image-container">
                                <img class="image" :src="image.src" :alt="image.alt" :class="image.category"
                                    v-show="showImage(image.category)" @click="openModal(index)">
                            </div>
                            <div v-if="showModal" class="modal" tabindex="-1" role="dialog">
                                <div class="modal-dialog modal-dialog-centered" role="document">
                                    <div class="modal-content">
                                        <div class="modal-header">
                                        </div>
                                        <div class="modal-body d-flex align-items-center">
                                            <span class="w3-display-left w3-btn" @click="plusDivs(-1)">
                                                <i class="fas fa-angle-left"></i></span>

                                            <img :src="images[currentIndex].src" class="img-fluid" alt="Modal Image">

                                            <span class="w3-display-right w3-btn" @click="plusDivs(1)">
                                                <i class="fas fa-angle-right"></i></span>
                                        </div>
                                    </div>
                                </div>
                                <div class="btn-x w3-text-white w3-xxlarge w3-hover-text-grey w3-container me-5"
                                    @click="closeModal" style="cursor:pointer">x</div>
                            </div>
                        </div>

                    </div>
                </div>
                
                     
            </div>
        </div> 
        <!-- <div class="brush_2 animate__animated animate__fadeInRight"><img src="https://marketifythemes.net/html/dizme/img/brushes/portfolio/2.png" alt /></div> --> 
    </section>


</template>


<script>


export default {
    name: "PortfolioComponent",

    data() {
        return {

            images: [
                { src: require('@/assets/cristal.jpg'), alt: 'Immagine 1', category: 'youtube' },
                { src: require('@/assets/moon.webp'), alt: 'Immagine 2', category: 'vimeo' },
                { src: require('@/assets/rings.webp'), alt: 'Immagine 3', category: 'soundcloud' },
                { src: require('@/assets/robot.jpg'), alt: 'Immagine 4', category: 'popup' },
                { src: require('@/assets/flower.jpg'), alt: 'Immagine 5', category: 'detail' },
                { src: require('@/assets/vortex.jpg'), alt: 'Immagine 6', category: 'popup' }

            ],
            currentCategory: 'all',
            showModal: false,
            currentIndex: 0

        };
    },
    methods: {

        filterImages(category) {
            this.currentCategory = category;
        },
        showImage(category) {
            return this.currentCategory === 'all' || category === this.currentCategory;
        },
        openModal(index) {
            this.showModal = true;
            this.currentIndex = index;
        },
        closeModal() {
            this.showModal = false;
        },
        plusDivs(n) {
            this.currentIndex += n;
            if (this.currentIndex >= this.images.length) {
                this.currentIndex = 0;
            }
            if (this.currentIndex < 0) {
                this.currentIndex = this.images.length - 1;
            }
        },
        currentDiv(n) {
            this.currentIndex = n;
        }
    },


    created() {
        this.filterImages('all');
    }








};





</script>





<style scoped>



span {
    color: #f75023;
    font-size: 22px;
    font-family: 'Jost', sans-serif;
    font-weight: 600;

}

h3 {
    font-size: 40px;
    font-family: 'Jost', sans-serif;
    font-weight: 500;
    color: white;
}

p {
    color: #706f7c;
    font-family: 'Jost', sans-serif;
    font-size: 18px;
    font-weight: 500;

}



.filter ul li.current a {
    color: #f75023
}

.filter ul li a:hover {
    color: #f75023
}


.filter ul li a:before {
    color: #f75023
}

.filter ul li .a.current {
    color: #f75023
}

.filter ul li .a:hover {
    color: #f75023
}

.filter ul li {
    margin: 0px 50px 0px 0px;
    display: inline-block;
    font-family: 'Jost', sans-serif;
    font-weight: 500;
    border: none;
    list-style-type: none;
    padding-top: 5%;
    padding-bottom: 5%;
    transform: scale(1) translateZ(0);
    -webkit-transition: all .3s ease-in-out;
    -moz-transition: all .3s ease-in-out;
    -ms-transition: all .3s ease-in-out;
    -o-transition: all .3s ease-in-out;
    transition: all .3s ease-in-out;
    cursor: pointer;

}



.filter ul li:last-child {
    margin-right: 0
}


a {
    text-decoration: none;
    color: white;
}


.gallery {
    width: 1160px;
    margin: 0 auto;
}


.grid-container {
    display: grid;
    grid-auto-flow: dense;
    gap: 30px;
    grid-template-columns: repeat(minmax(300px, 1fr));
    justify-content: center;
    align-content: center;
    grid-template-areas:
        "image-0 image-1 image-4"
        "image-0 image-3 image-4 "
        "image-2 image-3 image-5 "
        "image-2 image-3 image-5"
        "image-2 image-3 image-5";
      
}

.grid-container img{
    width: 100%;
    height:100%;
    position: relative;
    overflow: hidden;
    border-radius: 12px;
    
}




.image-container:hover img{
    transform: scale(1.1) ;
    transition: all .3s ease-in-out;
    transition: all .2s linear; 
       
    
}


.image-container {
    position: relative;
    overflow: hidden;
    display: block;
    border-radius: 12px; 
   
}




.image-0 {
    grid-area: image-0;
}

.image-1 {
    grid-area: image-1;
}

.image-2 {
    grid-area: image-2;
}

.image-3 {
    grid-area: image-3;
}

.image-4 {
    grid-area: image-4;
}

.image-5 {
    grid-area: image-5;
}



.modal-header {
    border-bottom: none;
}

.modal {
    background: rgba(0, 0, 0, 0.721);
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    scrollbar-width: none;
    
}

.modal::-webkit-scrollbar {
    display: none;
    
}


.modal-dialog {
    max-width: 90%;

}

.modal-content {
    background-color: transparent;
    border: none;

}

.fa-angle-right,
.fa-angle-left {
    font-size: 22px;
    color: white;
    /* border-radius: 50%; */
    /* border: 2px solid white; */
    height: 45px;
    width: 45px;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    position: fixed;
}


.modal-body img {
    object-fit: none;
}

.modal-body {
    min-width: 92vw;
    min-height: 30vh;
    overflow: hidden;
    display: flex;
    align-items: center;
    position: relative;
}





.btn-x {
    top: 0;
    transform: translateY(-250px);
    font-size: 20px;
    color: white;
    display: flex;
    justify-content: center;
    align-items: center;
    background: transparent;
    border-radius: 50%;
    width: 50px;
    height: 50px;
    z-index: 100;
    text-align: center;
    line-height: 50px;
}


.brush_1 {
    left: 0px;
    transform: translateY(180px);
    margin-left: -60px;
    padding: 0;
    }

.brush_2 {
    position: absolute;
    left: 60%;
    margin-left: 100px;
    

}
    



/* 
.zoom-container {
    display: inline-block;
    overflow: hidden;
}

.zoom-image {
    width: 100%;
    height: auto;
    transition: transform 0.3s ease-in-out;
} */
</style>