<script setup lang="ts">
import part2 from '../styles/part2.module.css'
const ButtonWebflowContent = "View on Webflow"
const LinkConect = "contact Us"

</script>
<template>
    <div :class="part2.ButtonCollection">
        <div :class="part2.ButtonWebflow"><button :src=ButtonWebflowContent :class="part2.ButtonWebflow">{{ButtonWebflowContent}}</button></div>
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


