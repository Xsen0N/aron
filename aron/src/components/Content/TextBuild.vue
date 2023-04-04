<script setup lang="ts">
import part2 from '../styles/part2.module.css'
const BuildText = "BUILD"
const Adjective = "fantastic"
const WebflowText = "WEBFLOW WEBSITES"
//import '../styles/part2.css'
</script>
<template>
    <div  :class="part2.FirstRowTextBuild">
        <h3 :src=BuildText :class="part2.BuildText">{{BuildText}}
    <div :src=Adjective :class="part2.Adjective">{{Adjective}}</div></h3>
    <div :class="part2.AdjectiveLine"></div>
    </div>
    <h3 :src=WebflowText :class="part2.WebflowText">{{WebflowText}}</h3>
</template>

