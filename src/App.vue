<template>
  <div>
  <HeaderComponent/>
  <JumboComponent/>
  <MainComponent/>
  <FooterComponent/>
  </div>
</template>

<script>

import HeaderComponent from './components/HeaderComponent.vue'
import JumboComponent from './components/JumboComponent.vue'
import MainComponent from './components/MainComponent.vue'
import FooterComponent from './components/FooterComponent.vue'

export default {
  name: 'App',
  components: {
    HeaderComponent,
    JumboComponent,
    MainComponent,
    FooterComponent,

  }
}
</script>

<style>

@import url("https://fonts.googleapis.com/css2?family=Jost:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;1,300;1,400;1,500;1,600;1,700;1,800&display=swap");






#app {
  box-sizing: border-box ;
  font-family: 'Jost'sans-serif;
  font-weight: 16px;
  text-align: justify content;
  color: white;
  background-color:#2b2d33;
  background-image:url(https://marketifythemes.net/html/dizme/img/slider/2.jpg);
  background-repeat: no-repeat;
  background-size: contain;
  background-position: center top;
  margin: 0;
  padding: 0;
  width: 100%;
  overflow-x: hidden; /* Nasconde lo scroll orizzontale */


  
 

::-webkit-scrollbar {
width: 10px; /* Larghezza della barra di scorrimento */
}

/* Stile per il track della barra di scorrimento */
::-webkit-scrollbar-track {
 background: grey; /* Colore di sfondo del track */
}

/* Stile per il thumb della barra di scorrimento */
::-webkit-scrollbar-thumb {
 background: black; /* Colore del thumb */
}

/* Stile per il thumb quando si passa il mouse sopra */
::-webkit-scrollbar-thumb:hover {
 background: black; /* Colore del thumb al passaggio del mouse */
}





 
  
 
  }
h1,
h2,
h3,
h4,
h5,
h6 {
    font-weight: 500;
    line-height: 1.3;
    font-family: jost, sans-serif;
    color: #000
}


h1 {
    font-size: 45px
}

h2 {
    font-size: 36px
}

h3 {
    font-size: 30px
}

h4 {
    font-size: 24px
}

h5 {
    font-size: 20px
}

h6 {
    font-size: 16px
}




.container {
 width: 100%; /* Assicura che il contenitore occupi tutta la larghezza disponibile */
 max-width: 100%; /* Previene che il contenitore superi la larghezza della finestra */
}



</style>
