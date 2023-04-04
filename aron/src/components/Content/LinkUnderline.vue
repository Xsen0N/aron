<script lang="ts">
import part2 from '../styles/part2.module.css'
export default {
    props: {
        LinkConect: String, 
    }
  }
</script>

<template>
        <a :src=LinkConect class="LinkConect">
            <div class="LinkAnimate">
                <div>{{LinkConect}}</div>
                <div class="LinkConectLine"></div>
            </div>
        </a>
</template>

<style>
.LinkConect{
  display: inline;
  position: relative;
  color: #d6d1ca;
  font-family: 'Source Sans 3', sans-serif;
  text-transform: uppercase;
  text-decoration: none;
  font-size: 14px;
  margin-left: 40px;
  margin-top: 15px;
}

.LinkConectLine{
  position: relative;
  width: 100%;
  height: 1px;
  background-color: #4a524a;
  
}
.LinkConectLine::after {
  content: '';
  display: block;
  width: 0;
  height: 2px;
  background-color: #000;
  transition: width 0.3s, background-color 0.3s;
}

.LinkAnimate:hover .LinkConectLine::after {
  width: 100%;
  color: #000;
  background-color: #ffea00;
}

.LinkAnimate:hover {
  color: #ffea00;
}
</style>