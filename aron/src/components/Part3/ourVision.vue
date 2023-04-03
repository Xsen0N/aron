<template>
    <section :class="styles.main_sec">
        <photoComp/>
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

<script>
//import photoComp from "../photoComponent/photoComp.vue";
import styles from "../styles/ourVision.module.css";


</script>

<style>
</style>