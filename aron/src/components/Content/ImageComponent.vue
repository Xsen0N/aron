
<template>
  <h3 class="ClientText" :style="ClientTextstyles">{{text}}</h3>
  <div class="ComboTextPhoto">
    <img :src=imageSrc :style="ClientImagestyles"/>
    <h3 class="ClientText2" :style="ClientText2styles">{{text}}</h3>
  </div>
</template>
<script lang="ts">
export default {
  props: {
    imageSrc: String,
    text: String,
    ClientTextstyles: Object,
    ClientText2styles: Object,
    ClientImagestyles: Object
  }
}
</script>

<style>


.ClientText{
  z-index: 0;
  opacity: 1;
  position: absolute;
  text-align: center;
  vertical-align: middle;
  color:#d6d1ca;
  font-family: 'Source Sans 3', sans-serif;
  text-transform: uppercase;
  font-size: 94px;
  margin-left: -36px;
  margin-top: 233px;
  background: none;

}
.ComboTextPhoto{
  position: relative;
  display: flex;
  overflow: hidden;
  max-width: 100%;
  margin-right: auto;
  margin-left: auto;
  align-items: center
}
.ClientText2{
  z-index: 2;
  color: #ffea00;
  font-family: 'Source Sans 3', sans-serif;
  text-transform: uppercase;
  font-size: 94px;
  opacity: 1;
  position: absolute;
  text-align: center;
  vertical-align: middle;
  background: none;
}
</style>
