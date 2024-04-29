<template>
    <section class="dizme_map">
        <div class="mapouter">
            <div class="gmap"><iframe width="1000" height="375" style="border-radius:12px" id="gmap_canvas"
                    src="https://maps.google.com/maps?q=2880%20Broadway,%20New%20York&t=&z=13&ie=UTF8&iwloc=&output=embed"
                    frameborder="0" scrolling="no" marginheight="0" marginwidth="0"></iframe><a
                    href="https://123movies-a.com"></a><br>

            </div>
     
        </div>
        
    </section>

</template>


<script>


export default {
    name: "MapComponent",
}

</script>

<style scoped>
.mapouter {
    position: relative;
    text-align: center;

}

.gmap {
    overflow: hidden;
    background: none;
    padding-bottom: 200px;

}
</style>