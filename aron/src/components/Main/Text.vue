<script setup lang="ts">
import {ref,defineProps} from 'vue'
const WeDoImg = "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61ba12b6a7ce351d1a5245b8_photo-1.jpg"
const philosopy_text ="What we do"
const firstline = "aron creates"
const secondline = "innovation "
const secondline2 = "by design"
const thirdline = "not by chance."
import texts from '../styles/texts.module.css'
const props = defineProps({
    creates:Array
    })
</script>
<template>
<div :class="texts.block2">

    <div :class="textstext_wrapper">
        <div :class="textsphoto_animation_page">
<div class="itemBrandPhoto">
                <ImageComponent :text="text" :imageSrc="imageSrc" :ClientImagestyles="ClientImagestyles" :ClientTextstyles="ClientTextstyles" :ClientText2styles="ClientText2styles"/>

      </div>
        </div>
    </div>
<div :class="texts.maincolomn" id="myAnchor">
        <div :class="texts.table">
             <p :src="firstline" :class="texts.line">{{firstline}}</p>
             <p :src="secondline" :class="texts.line"><span :src="secondline" :id="texts.inov" > {{secondline}}</span>{{secondline2}} </p>
             <p :src="thirdline" :class="texts.line"> {{thirdline}} </p>
         </div>

    <div :class="texts.secondcolumn">
        <div :class="texts.textprops" v-for="(item,newkey) in props.creates" :key="newkey">
              <img :src=item.img :class="texts.icons"> 
              <div :class="texts.maintext"> {{item.maintext}}</div>
              <div :class="texts.addettext"> {{item.text}}</div>
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
        'margin-left': '-79px',
        'margin-top': '29px' },
      ClientImagestyles: { 
        'width': '100%',
        'height': '100%',
        'object-position': '50% 0%'}
    }
  }
}
</script>
