<template>
    <footer>
        <modal v-if="showModal" @close="closeModal"/>
        <section :class="styles.first_sec">
            <div :class="styles.main_text1">READY TO TALK</div>
            <div :class="styles.main_text2">FEEL FREE TO WRITE US.</div>
            <div :class="styles.buttons">
                <button v-on:click="callModal()" :class="styles.but_contact">Contact Us</button>
                <button  :class="styles.but_call">MAKE A CALL</button>
            </div>
        </section>
        <section :class="styles.second_sec">
            <div :class="styles.list">
                <ul>
                    <li>HOME</li>
                    <li>ABOUT</li>
                    <li>PRICING</li>
                    <li>NEWS</li>
                    <li>CONTACT</li>
                </ul>
            </div>
            <div :class="styles.row2">
                <div :class="styles.hq">HQ ADDRESS</div>
                <div :class="styles.addr">741 New South Head Rd, Triple Bay SWFW 3148, New York</div>
                <div :class="styles.cont">CONTACT</div>
                <div :class="styles.mail">HELLO@ARON.COM</div>
                <div :class="styles.tel">+1 317 711 105</div>
            </div>
            <div :class="styles.row3">
                <div :class="styles.foll">FOLLOW US</div>
                <div :class="styles.style">STYLE GUIDE</div>
                <div :class="styles.imag">IMAGE LICESING</div>
                <div :class="styles.powered">© This is a Deni Bozo template powered by Webflow</div>
            </div>
        </section>
    </footer>
</template>

<script>
import styles from "./styles/footer.module.css";
import modal from "./modal.vue";

export default {
    data() {
        return {
            styles,
            showModal: false,
        }
    },

    components: {
        modal
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

 
<style module>

</style>