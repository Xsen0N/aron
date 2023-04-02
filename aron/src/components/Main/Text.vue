<script setup lang="ts">
import {ref,defineProps} from 'vue'
const WeDoImg = "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61ba12b6a7ce351d1a5245b8_photo-1.jpg"
const philosopy_text ="What we do"
const firstline = "aron creates"
const secondline = "innovation "
const secondline2 = "by design"
const thirdline = "not by chance."
import '../styles/text.css'
const props = defineProps({
    creates:Array
    })
</script>
<template>
<div class="block2">

    <div class="text_wrapper">
        <div class="photo_animation_page">
            <img :src=WeDoImg class="WeDoImg">
            <h3 :src=philosopy_text class="philosopy_text">{{philosopy_text}}</h3>
             <div class="absolute-background"></div>
        </div>
    </div>
<div class="maincolomn">
        <div class="table">
             <p :src="firstline" class="line">{{firstline}}</p>
             <p :src="secondline" class="line"><span :src="secondline" class="inov" > {{secondline}}</span>{{secondline2}} </p>
             <p :src="thirdline" class="line"> {{thirdline}} </p>
         </div>

    <div class="secondcolumn">
        <div class="textprops" v-for="(item,newkey) in props.creates" :key="newkey">
              <img :src=item.img class="icons"> 
              <div class="maintext"> {{item.maintext}}</div>
              <div class="addettext"> {{item.text}}</div>
        </div>  
    </div>
</div>
</div>
</template>
