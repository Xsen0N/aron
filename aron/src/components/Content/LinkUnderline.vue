<script lang="ts">
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