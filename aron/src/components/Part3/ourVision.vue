<template>
    
    <div :class="styles.imageCompContainer">
        <ImageComponent v-bind:ClientImagestyles="photoContainer" image-src="https://assets.website-files.com/61b88a38b30a977e957e8ca7/61bb356a67fcdb2f66fac720_photo-5-p-500.jpeg"  text="Our vision"/>
    </div>
    <section :class="styles.main_sec">
        <!-- <photoComp/> -->
        <div :class="styles.text">
            <div :class="styles.text_m">
                WE WORRY ABOUT<br/> THE DETAILS SO YOU<br/> DON'T HAVE TO.
            </div>
            <div :class="styles.text_about">
                What makes Aron Studio unique is our vision. When we first started as
                a design agency, we made a promise to ourselves to honor our creative
                impulses.
            </div>
            <button :class="styles.button">More About Us</button>
        </div>
        <div :class="styles.line"></div>
    </section>
</template>

<script setup lang="ts">
import styles from "../styles/ourVision.module.css";
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

// export default {
// // data() {
// //     return {
// //         photoName = "../../assets/girl.jpg",
// //         photoText = "OUR VISION",
// //     },
// // },
//     data() {
//         return {
//             styles
//         }
//     },

    // components: {
    //     photoComp
    // },

</script>

<style>
.photoContainer {
    position: relative;
    bottom: 35px;
}
</style>