<script setup lang="ts" >
import part2 from '../styles/part2.module.css'
const itemText1 = "We worked with the world’s"
const SubItemText = " Biggest "
const itemText2 = "Brands "
const BrandItem1 = "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61bb2c61fe2f6ce01965bb09_logo-7.png"
const BrandItem2 = "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61bb2c60e9c0ac958a85d041_logo-4.png"
const BrandItem3 = "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61bb2d516f46359b2f65ff5f_logo-1.png"
const BrandItem4 = "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61bb2cee18572452404af6fa_logo-2.png"
const BrandItem5 = "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61bb2bf3f6568fe42760793e_logo-6.png"
const BrandItem6 = "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61bb2c6006e6f7e256ba18cc_logo-8.png"
const ButtonEnquireUs = "Enquire Us";

</script>
<template>
    <div :class="part2.gridContainerClient" id="workwithus">
      <div :class="part2.itemList">
        <p :src=itemText1 :class="part2.itemText1">{{itemText1}}</p>
        <span :src=SubItemText :class="part2.SubItemText">{{SubItemText}}</span>
        <p :src=itemText2 :class="part2.itemText2">{{itemText2}}</p>
        </div>
      <div :class="part2.listOfBrands">
        <div :class="part2.BrandItem1"><img :src=BrandItem1 :class="part2.BrandItem1"/></div>
        <div :class="part2.BrandItem2"><img :src=BrandItem2 :class="part2.BrandItem2"/></div>
        <div :class="part2.BrandItem3"><img :src=BrandItem3 :class="part2.BrandItem3"/></div>
        <div :class="part2.BrandItem4"><img :src=BrandItem4 :class="part2.BrandItem4"/></div>
        <div :class="part2.BrandItem5"><img :src=BrandItem5 :class="part2.BrandItem5"/></div>
        <div :class="part2.BrandItem6"><img :src=BrandItem6 :class="part2.BrandItem6"/></div>
        <button :src=ButtonEnquireUs :class="part2.ButtonEnquireUs">{{ButtonEnquireUs}}</button>
      </div>
      <div :class="part2.itemBrandPhoto">
        <ImageComponent :text="text" :imageSrc="imageSrc" :ClientImagestyles="ClientImagestyles" :ClientTextstyles="ClientTextstyles" :ClientText2styles="ClientText2styles"/>
      </div>
    </div>
</template>

<script lang="ts">
import ImageComponent from './ImageComponent.vue'
export default {
  components: {
    ImageComponent
  },
  data() {
    return {
      imageSrc: 'https://assets.website-files.com/61b88a38b30a977e957e8ca7/61bb24d6a1230404fc2678ff_photo-2.jpg',
      text: 'Our Client',
      ClientTextstyles: { },
      ClientText2styles: {    
        'width': '600px',
        'margin-left': '-74px',
        'margin-top': '96px' },
      ClientImagestyles: { 
        'width': '100%',
        'height': '100%',
        'object-position': '50% 0%'}
    }
  }
}
</script>