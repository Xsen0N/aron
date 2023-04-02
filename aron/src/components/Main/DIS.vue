<script setup lang="ts">
import {ref,defineProps} from 'vue'
import '../styles/dis.css'
const props = defineProps({
    items:Array
    })
const firstpart = "We are an award-winning branding "
const Andpart = "&"
const secondpart = " web studio committed to excellence since forever."
const treangle = "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61b9e026db2460fa1749d674_play_arrow_black_24dp.svg"
const downscrool = "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61b9e277e1f8a2db88a96334_scroll.png"
const play = "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61b9e248f608c4777d8b35b7_arrow_downward_black_24dp.svg" 
</script>

<template >
<div>
    <div>
    <div class="FAS"> 
        <p :src="firstpart" id="firstpart"> {{firstpart}} </p>
        <p :src="Andpart" id="Andpart"> {{Andpart}}  </p> 
        <p :src="secondpart" id="secondpart"> {{secondpart}} </p>   
     </div>
    </div>

    <div class="text" v-for="(item,key) in props.items" :key="key">
        {{item.word}}
    </div>


    <div>
<div id= "square1"><img :src ="treangle" class="pause"> </div>
    </div> 

    <div class="mainScroll"> 
         <img :src="play" class ="play"> 
        <div class="po"> <img :src="downscrool" class ="downscrool"> </div>
    </div> 


    
</div>
</template>
<style>
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display&family=Red+Hat+Mono:wght@300;400&display=swap');
</style>