<script setup lang="ts">
const ButtonWebflowContent = "View on Webflow"
const LinkConect = "contact Us"
import '../styles/part2.css'
</script>
<template>
    <div class="ButtonCollection">
        <div class="ButtonWebflow"><button :src=ButtonWebflowContent class="ButtonWebflow">{{ButtonWebflowContent}}</button></div>
        <LinkUnderline :LinkConect="LinkConect"/>
    </div>
</template>

<script lang="ts">
import LinkUnderline from './LinkUnderline.vue'
export default {
  components: {
    LinkUnderline
  },
  data() {
    return {
        LinkConect: 'contact Us'
    }
  }
}

</script>


