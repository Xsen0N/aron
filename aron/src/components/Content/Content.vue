<script setup lang="ts">
import part2 from '../styles/part2.module.css'
import ButtonWebflow from './ButtonWebflow.vue'
import BookImage from './BookImg.vue'
import TextBuild from './TextBuild.vue'

import GridClient from './GridClient.vue'
import ImageComponent from './ImageComponent.vue'
import Gallery from './Gallery.vue'
const prop = defineProps({
    ButtonWebflowContent :String,
    BookImage: String,
    ColorImage : String,
    BuildText : String,
    Adjective : String,
    WebflowText : String,
    LinkConect: String,
    ClientText: String,
    imgSrc:String,
    Capture:String
})

</script>

<template>
  
    <div :class= "part2.ImageBook_wrapper">
        <BookImage/>
    </div>
    <div :class= "part2.TextBuild_wrapper">
        <TextBuild/>
    </div>
    <div :class= "part2.button_wrapper">
        <ButtonWebflow/>
    </div>
    <div :class= "part2.GridClient_wrapper">
        <GridClient/>
    </div>
    <div :class= "part2.Gallery_wrapper">
        <Gallery/>
    </div>
</template>

<script lang="ts">

export default {
  components: {
    ImageComponent
  },
  data() {
    return {
      imageSrc: 'https://assets.website-files.com/61b88a38b30a977e957e8ca7/61bb24d6a1230404fc2678ff_photo-2.jpg',
      text: 'Our Client'
    }
  }
}
</script>