<script setup lang="ts">
import {ref,defineProps} from 'vue'
import first from '../styles/first.module.css'
const Aron = "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61b9cec5a0137701a8068e4e_logo.png"
const Pack = "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61b9cc9aac7d37458cf93dae_local_mall_black_24dp.svg" 
const enquire = "enquire us:"

function reloadPage() {
      window.location.href = '/';
    }


</script>
<template>
<header :class="first.main"> 
    <div :class="first.aron" @click="reloadPage"> <img :src=Aron :id="first.aron_logo" ></div>
    <div :id="first.slash"> </div>
    <div :src =enquire :id= "first.eu"> {{enquire}} </div>
<div>
    <div :src=Hello :id="first.hello"> <LinkUnderline :LinkConect="LinkConect"/> </div>
    <div :class="first.buttonLine"> 
            <div :class="first.buttonLineAbs" > </div> 
    </div> 
</div> 

<div :id="first.pac">
<img :src=Pack :class="first.Aron">
</div> 
<div :id= "first.square"> 0 </div>
<div>
    <div :id= "first.topline">  </div>
    <div :id= "first.btnline"> </div> 
</div> 
</header> 
<hr/>
</template>

<script lang="ts">
import LinkUnderline from '../Content/LinkUnderline.vue'
export default {
  components: {
    LinkUnderline
  },
  data() {
    return {
        LinkConect: 'Hello@aron.com'
    }
  }
}

</script>