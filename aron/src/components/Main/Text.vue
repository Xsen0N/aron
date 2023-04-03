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
<div class="itemBrandPhoto">
                <ImageComponent :text="text" :imageSrc="imageSrc" :ClientImagestyles="ClientImagestyles" :ClientTextstyles="ClientTextstyles" :ClientText2styles="ClientText2styles"/>

      </div>
        </div>
    </div>
<div class="maincolomn" id="myAnchor">
        <div class="table">
             <p :src="firstline" class="line">{{firstline}}</p>
             <p :src="secondline" class="line"><span :src="secondline" id="inov" > {{secondline}}</span>{{secondline2}} </p>
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

<script lang="ts">
import ImageComponent from '../Content/ImageComponent.vue'
export default {
  components: {
    ImageComponent
  },
  data() {
    return {
      imageSrc: 'https://assets.website-files.com/61b88a38b30a977e957e8ca7/61ba12b6a7ce351d1a5245b8_photo-1.jpg',
      text: 'What we do',
    ClientTextstyles: { },
      ClientText2styles: {    
        'width': '692px',
        'margin-left': '-74px',
        'margin-top': '30px' },
      ClientImagestyles: { 
        'width': '100%',
        'height': '100%',
        'object-position': '50% 0%'}
    }
  }
}
</script>
