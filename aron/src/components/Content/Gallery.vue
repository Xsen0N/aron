<script setup lang="ts">
import part2 from '../styles/part2.module.css'
const image1 = "./image1.png"
const image2 = "./image2.png"
const image3 = "./image1.png"
const textGallery = 'WHAT THEY '
const textThink = 'THINK'
</script>
<template>
<h3 class="textGallery">{{ textGallery }} <span :class="part2.textThink">{{ textThink }}</span></h3>
    <div class="gallery">
 
  <div class="gallery__item">
    <img src="./image1.png" alt="image1">
  </div>
  <div class="gallery__item">
    <img src="./image2.png" alt="image2">
  </div>
  <div class="gallery__item">
    <img src="./image3.png" alt="image3">
  </div>
</div>
</template>

<style>
.gallery {
  display: flex;
  justify-content: space-between;
}

.gallery__item {
  position: relative;
  flex-basis: calc(33.33% - 10px);
  margin-right: 10px;
  transition: transform 0.3s, opacity 0.3s ;
}

.gallery__item:hover {
  transform: translateY(-10px);
  opacity: 1;
  z-index: 1;
}

.gallery__item img {
  width: 100%;
  opacity: 0.6;
  transition: opacity 0.3s;
}

.gallery__item:hover img {
  opacity: 1;
}


.gallery__item:hover:before {
  padding-bottom: calc(100% + 10px);
}

.textGallery{
  text-align: left;
  font-family: 'Source Sans 3';
    font-style: normal;
    font-weight: 400;
    font-size: 50px;
    line-height: 50px;
    text-transform: uppercase;
    color: #D6D1CA;
    padding-bottom: 40px;
}

</style>

