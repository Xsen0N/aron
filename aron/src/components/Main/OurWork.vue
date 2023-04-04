<script setup lang="ts">
import block from '../styles/block.module.css';
import {ref,defineProps} from 'vue'
const props = defineProps({
    texts:Array
    })
//import '../styles/work.css'
const work = "Our Work"
const workwithus = "work with us"
const scrollToWorkBlock = (anchor: string) => {
  const anchorEl = document.querySelector(anchor)
  if (anchorEl) {
    anchorEl.scrollIntoView({ behavior: 'smooth' })
  }
}
</script>

<styles module>
  
</styles>

<template>
<div :class="block.lastblock">
<div :class="block.firstblock">
  
       <div  :src ="work"  :class="block.work"> {{work}} </div >
       <div :src ="workwithus " :class="block.work2" @click="scrollToWorkBlock('#workwithus')">  <LinkUnderline :LinkConect="LinkConect"/></div >
   
</div>
    <div :class="block.words" v-for="(part,keys) in props.texts" :key="keys">
        {{part.part}}
    </div>
</div>
</template>

<script lang="ts">
import LinkUnderline from '../Content/LinkUnderline.vue'
export default {
  name: 'OurWork',
  components: {
    LinkUnderline
  },
  data() {
    return {
        LinkConect: 'work with us'
    }
  }
}

</script>