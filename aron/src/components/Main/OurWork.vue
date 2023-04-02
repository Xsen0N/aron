<script setup lang="ts">
import {ref,defineProps} from 'vue'
const props = defineProps({
    texts:Array
    })
import '../styles/work.css'
const work = "Our Work"
const workwithus = "work with us"
</script>
<template>
<div>
<div class="firstblock">
  
       <div  :src ="work"  class="work"> {{work}} </div >
       <div :src ="workwithus " class="work2">  {{workwithus}}</div >
   
</div>
    <div class="words" v-for="(part,keys) in props.texts" :key="keys">
        {{part.part}}
    </div>
</div>
</template>