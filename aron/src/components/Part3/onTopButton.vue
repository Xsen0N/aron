<template>
    
    <div ref="onTopBut" class="onTopContainer" id="strelka_container">
    <a @click="topBut" id="onTop" href="#">
        <svg class="strelka-top-4" width="17" height="17" viewBox="0 0 17 17" fill="none" xmlns="http://www.w3.org/2000/svg">
    <path d="M16.1666 8.49998L14.8154 7.14873L9.45831 12.4962V0.833313H7.54165V12.4962L2.19415 7.13915L0.833313 8.49998L8.49998 16.1666L16.1666 8.49998Z" fill="#cccccc"/>
    </svg>
    </a>
    </div>
   
</template>

<script>
// import styles from "../styles/onTop.module.css";

export default { 

    methods: {
        vueOnScroll() {
            var prev = window.pageYOffset;
            const refs = this.$refs.onTopBut;
            window.addEventListener("scroll", () => {
                var curr = window.pageYOffset;
                if(curr > prev) {
                    refs.classList.add("appear");
                    refs.classList.remove("disappear");
                }
                if(curr < prev) {
                    refs.classList.add("disappear");
                    refs.classList.remove("appear");
                }
                prev = curr;
            })
        },

        topBut() {
            const anchor = document.querySelector("#onTop");
            anchor.addEventListener("click", (event)=> {
                event.preventDefault();
                document.querySelector("body").scrollIntoView({
                    behavior: "smooth",
                    block: "start"
                })
            })
        }
    },

    mounted() {
        // run the function when the component's mount
        this.vueOnScroll();
    }
}

</script>

<style>
@import '../styles/onTop.css';
</style>