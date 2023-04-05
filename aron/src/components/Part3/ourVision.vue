<template>
    <section class="main_sec">
        <div class="imageCompContainer">
            <ImageComponent image-src="https://assets.website-files.com/61b88a38b30a977e957e8ca7/61bb356a67fcdb2f66fac720_photo-5-p-500.jpeg"  text="Our vision"/>
        </div>
        
        <div class="text">
            <div class="text_m">
                WE WORRY ABOUT<br/> THE <span class="details">DETAILS</span> SO YOU<br/> DON'T HAVE TO.
            </div>
            <div class="text_about">
                What makes Aron Studio unique is our vision. When we first started as
                a design agency, we made a promise to ourselves to honor our creative
                impulses.
            </div>
            <button class="button">More About Us</button>
        </div>
        <div class="line"></div>
    </section>
</template>

<script setup lang="ts">
import ImageComponent from "../Content/ImageComponent.vue";

// new Vue({
//     el: '#APP3',
//     name: "ourVision",
//     components: {
//         ImageComponent
//     },

//     data() {
//         return {
//             imageSrc: "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61bb356a67fcdb2f66fac720_photo-5-p-500.jpeg",
//             text: "OUR VISION",
//         }

//     }

// }
// );
//let styles : any;


</script>

<style>
@import '../styles/ourVision.css';
</style>