<script setup lang="ts">
const BuildText = "BUILD"
const Adjective = "fantastic"
const WebflowText = "WEBFLOW WEBSITES"
//import '../styles/part2.css'
</script>
<template>
    <div  class="FirstRowTextBuild">
        <h3 :src=BuildText class="BuildText">{{BuildText}}
    <div :src=Adjective class="Adjective">{{Adjective}}</div></h3>
    <div class="AdjectiveLine"></div>
    </div>
    <h3 :src=WebflowText class="WebflowText">{{WebflowText}}</h3>
</template>

