<script setup lang="ts">
const BuildText = "BUILD"
const Adjective = "fantastic"
const WebflowText = "WEBFLOW WEBSITES"
import '../styles/part2.css'
</script>
<script lang="ts">





</script>
<template>
    <div  class="FirstRowTextBuild">
        <h3 :src=BuildText class="BuildText">{{BuildText}}
    <div :src=Adjective class="Adjective">{{Adjective}}</div></h3>
    <div class="AdjectiveLine" v-show="showLine" :style="{backgroundColor: adjColor}"></div>
    </div>
    <h3 :src=WebflowText class="WebflowText">{{WebflowText}}</h3>
</template>

<style>
.Adjective {
  display: inline-block;
  overflow: hidden;
  animation: typing 4s steps(50, end) 1s forwards;
}

@keyframes typing {
  from {
    width: 0;
  }
  to {
    width: 100%;
  }
}
</style>