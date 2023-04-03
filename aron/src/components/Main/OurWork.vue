<script setup lang="ts">
import {ref,defineProps} from 'vue'
const props = defineProps({
    texts:Array
    })
import '../styles/work.css'
const work = "Our Work"
const workwithus = "work with us"
const scrollToWorkBlock = (anchor: string) => {
  const anchorEl = document.querySelector(anchor)
  if (anchorEl) {
    anchorEl.scrollIntoView({ behavior: 'smooth' })
  }
}
import block from '../styles/block.module.css';
</script>


<template>
<div class="lastblock">
<div class="firstblock">
  
       <div  :src ="work"  class="work"> {{work}} </div >
       <div :src ="workwithus " class="work2" @click="scrollToWorkBlock('#workwithus')">  <LinkUnderline :LinkConect="LinkConect"/></div >
   
</div>
    <div class="words" v-for="(part,keys) in props.texts" :key="keys">
        {{part.part}}
    </div>
</div>
</template>

<script lang="ts">
import LinkUnderline from '../Content/LinkUnderline.vue'
export default {
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