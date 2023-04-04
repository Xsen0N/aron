<script setup lang="ts">
import {ref,defineProps} from 'vue'
import dis from '../styles/dis.module.css'
const props = defineProps({
    items:Array
    })
const firstpart = "We are an award-winning branding "
const Andpart = "&"
const secondpart = " web studio committed to excellence since forever."
const treangle = "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61b9e026db2460fa1749d674_play_arrow_black_24dp.svg"
const downscrool = "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61b9e277e1f8a2db88a96334_scroll.png"
const play = "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61b9e248f608c4777d8b35b7_arrow_downward_black_24dp.svg" 

const videoId = ref('123456') // ID видео   
function playVideo() {
  window.open(`https://www.youtube.com/watch?v=ZOanF9DfDu0&t=3s&ab_channel=Webflow/watch?v=${videoId.value}`, '_blank')
}

const scrollToAnchor = (anchor: string) => {
  const anchorEl = document.querySelector(anchor)
  if (anchorEl) {
    anchorEl.scrollIntoView({ behavior: 'smooth' })
  }
}
</script>

<template >
<div>
    <div>
    <div :class="dis.FAS"> 
        <p :src="firstpart" :id="dis.firstpart"> {{firstpart}} </p>
        <p :src="Andpart" :id="dis.Andpart"> {{Andpart}}  </p> 
        <p :src="secondpart" :id="dis.secondpart"> {{secondpart}} </p>   
     </div>
    </div>

    <div :class="dis.text" v-for="(item,key) in props.items" :key="key">
        {{item.word}}
    </div>


    <div>
<button :id= "dis.square1" @click="playVideo"><img :src ="treangle" :class="dis.pause"> </button>
    </div> 

    <div :class="dis.mainScroll"> 
      <a @click="scrollToAnchor('#myAnchor')" >   <img :src="play" :class ="dis.play" > </a>
        <div :class="dis.po"> <img :src="downscrool" :class ="dis.downscrool"> </div>
    </div> 


    
</div>
</template>
<style>
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display&family=Red+Hat+Mono:wght@300;400&display=swap');
</style>

