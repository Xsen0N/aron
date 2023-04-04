<template v-on:scroll="check">
    <div>
        <ourVision/>
    </div>
    <div>
        <FooterBlock/>
    </div>
    <div>
        <onTopButton/>
    </div>

</template>

<script setup>
import ourVision from "./ourVision.vue";
import FooterBlock from "./FooterBlock.vue"
import onTopButton from "./onTopButton.vue"

</script>

<style >
@import url('https://fonts.googleapis.com/css2?family=Source+Sans+3:wght@200;300;400;500;600;700;800;900&display=swap');

* {
    font-family: 'Source Sans 3';

}
</style>