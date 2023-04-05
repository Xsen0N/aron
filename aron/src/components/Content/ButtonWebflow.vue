<script setup lang="ts">
import part2 from '../styles/part2.module.css'
const ButtonWebflowContent = "View on Webflow"
const LinkConect = "contact Us"

</script>
<template>
    <div :class="part2.ButtonCollection">
        <div :class="part2.ButtonWebflow"><button :src=ButtonWebflowContent :class="part2.ButtonWebflow">{{ButtonWebflowContent}}</button></div>
        <modal v-if="showModal" @close="closeModal"/>
        <LinkUnderline :LinkConect="LinkConect" v-on:click="callModal()" />
    </div>
</template>

<script lang="ts">
import LinkUnderline from './LinkUnderline.vue'
import modal from "../Part3/modal.vue";
export default {
  components: {
    LinkUnderline,
    modal
  },
  data() {
    return {
        LinkConect: 'contact Us',
        showModal: false,
    }
  },
  methods: {
        callModal() {
            this.showModal = true;
        },

        closeModal() {
            this.showModal = false;
        }
    }
}



</script>

