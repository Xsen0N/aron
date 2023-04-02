<script setup lang="ts">
import {ref} from 'vue'
import DIS from  './DIS.vue'
import first from './First.vue'
import Text from './Text.vue'
import OurWork from './OurWork.vue'
import '../styles/Main.css'
const items = ref([
      {word: "Digital", id: 1},
      {word:"Innovative", id: 2}, 
      {word:"Studio", id: 3}
])
const texts = ref([
      {part: "Pellente dapibus", id: 1},
      {part:"Consequat leo", id: 2}, 
      {part:"Auctor bortis", id: 3},
      {part:"Integer ante", id: 4},
      {part:"Etiam imdiet", id: 5},
      {part:"Cras ultricies", id: 6},
])
const prop = defineProps({
    WeDoImg: String,
    Aron: String,
    Pack: String,
    Hello: String,
    enquire: String,
    philosopy_text:String,
    work:String
})
const creates = ref([
    {img: "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61ba0d63adb67dee9ac606fc_icons8-sun-256.png", maintext: "STRATEGY", text:"Strategic masterplans and business/concept strategy"},
    {img: "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61ba0db82b87002983716dad_icons8-sale-price-tag-256.png", maintext: "ECOMMERCE", text:"High quality products that offer an all-in solution"},
    {img: "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61ba0d638fdd291d2562a339_icons8-feather-256.png", maintext: "DESIGN", text:"Standard of own film production that delivers"},
    {img: "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61ba146b363c2aebaad7a3d7_icons8-brain-256.png", maintext: "CONCEPT", text:"Award winning concepts and ideas from best team"},
])

</script>

<template>

<first/> 
    <DIS :items = "items"/>  
<Text :creates ="creates"/>
    <OurWork :texts = "texts"/> 
</template>