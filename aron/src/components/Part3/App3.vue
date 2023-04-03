<template v-on:scroll="check">
    <ourVision></ourVision>
    <FooterBlock></FooterBlock>
    <onTopButton></onTopButton>
</template>

<script>
import ourVision from "./ourVision.vue";
import FooterBlock from './FooterBlock.vue';
import onTopButton from './onTopButton.vue';

export default {
    name: "App",
    components: {
        ourVision, FooterBlock, onTopButton
    }
}



</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Source+Sans+3:wght@200;300;400;500;600;700;800;900&display=swap');

* {
    font-family: 'Source Sans 3';

}
</style>
