<script setup lang="ts">
import {ref,defineProps} from 'vue'
import '../styles/first.css'
const Aron = "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61b9cec5a0137701a8068e4e_logo.png"
const Pack = "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61b9cc9aac7d37458cf93dae_local_mall_black_24dp.svg" 
const Hello = "Hello@aron.com"
const enquire = "enquire us:"
</script>
<template>
<div class='main'> 

    <div id="aron"> <img :src=Aron id="aron-logo" ></div>
    <div id="slash"> </div>
    <div :src =enquire id= "eu"> {{enquire}} </div>
<div>
    <div :src=Hello id= "hello"> {{Hello}} </div>
    <div class="buttonLine"> 
            <div class="buttonLineAbs" > </div> 
    </div> 
</div> 

<div id="pac">
<img :src=Pack class="Aron">
</div> 
<div id= "square"> 0 </div>
<div>
    <div id= "topline">  </div>
    <div id= "btnline"> </div> 
</div> 
</div> 
<hr/>
</template>