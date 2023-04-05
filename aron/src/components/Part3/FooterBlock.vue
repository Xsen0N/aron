<template>
    <footer id="footer_container">
        <modal v-if="showModal" @close="closeModal"/>
        <section class="first_sec">
            <div class="main_text1">READY TO TALK</div>
            <div class="main_text2">FEEL FREE TO WRITE US.</div>
            <div class="buttons">
                <button v-on:click="callModal()" id="but_cont" class="but_contact">Contact Us</button>
                <LinkUnderline  v-bind:LinkConect="LinkConect"/>
                <!-- <button  class="but_call" >MAKE A CALL</button> -->
            </div>
        </section>
        <section class="second_sec">
            <div class="list">
                <ul>
                    <li>HOME</li>
                    <li>ABOUT</li>
                    <li>PRICING</li>
                    <li>NEWS</li>
                    <li>CONTACT</li>
                </ul>
            </div>
            <div class="row2">
                <div class="hq">HQ ADDRESS</div>
                <div class="addr">741 New South Head Rd, Triple Bay SWFW 3148, New York</div>
                <div class="cont">CONTACT</div>
                <div class="mail">HELLO@ARON.COM</div>
                <div class="tel">+1 317 711 105</div>
            </div>
            <div class="row3">
                <div class="foll">FOLLOW US</div>
                <div class="style">STYLE GUIDE</div>
                <div class="imag">IMAGE LICESING</div>
                <div class="powered">© This is a Deni Bozo template powered by Webflow</div>
            </div>
        </section>
    </footer>
</template>

<script lang="ts">
import modal from "./modal.vue";
import LinkUnderline from '../Content/LinkUnderline.vue';

export default {
    data() {
        return {
            showModal: false,
            LinkConect: 'Make a call'
        }
    },

    components: {
        modal, LinkUnderline
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
<!-- <script lang="ts">
export default {
  components: {
    
  },
  data() {
    return {
        LinkConect: 'Make a call'
    }
  }
}

</script> -->
 
<style>
@import '../styles/footer.css';
</style>