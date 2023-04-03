<script setup lang="ts">
import ButtonWebflow from './ButtonWebflow.vue'
import BookImage from './BookImg.vue'
import TextBuild from './TextBuild.vue'
import '../styles/part2.css'
import GridClient from './GridClient.vue'
import ImageComponent from './ImageComponent.vue'
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
  
    <div class= "ImageBook_wrapper">
        <BookImage/>
    </div>
    <div class= "TextBuild_wrapper">
        <TextBuild/>
    </div>
    <div class= "button_wrapper">
        <ButtonWebflow/>
    </div>
    <div class= "GridClient_wrapper">
        <GridClient/>
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