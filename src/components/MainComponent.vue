<template>
    <AboutComponent/>
    <PortfolioComponent/>
    <ProgressComponent/>
    <ServicesComponent/>
    <TestimonialsComponent/>
    <BlogComponent/>
    <SubscriveComponent/>
    <ContactComponent/>
    <MapComponent/>

    
    
</template>


<script>
import AboutComponent from './MainSections/AboutComponent.vue'
import PortfolioComponent from './MainSections/PortfolioComponent.vue'
import ProgressComponent from './MainSections/ProgressComponent.vue'
import ServicesComponent from './MainSections/ServicesComponent.vue'
import TestimonialsComponent from './MainSections/TestimonialsComponent.vue'
import BlogComponent from './MainSections/BlogComponent.vue'
import SubscriveComponent from './MainSections/SubscriveComponent.vue'
import ContactComponent from './MainSections/ContactComponent.vue'
import MapComponent from './MainSections/MapComponent.vue'



export default {
    name: "MainComponent",

    components:{
        AboutComponent,
        PortfolioComponent,
        ProgressComponent,
        ServicesComponent,
        TestimonialsComponent,
        BlogComponent,
        SubscriveComponent,
        ContactComponent,
        MapComponent,

    }
}

</script>

<style scoped>

</style>