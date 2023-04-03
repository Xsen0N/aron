<script setup lang="ts">
const ButtonWebflowContent = "View on Webflow"
const LinkConect = "contact Us"
import '../styles/part2.css'
</script>
<template>
    <div class="ButtonCollection">
        <div class="ButtonWebflow"><button :src=ButtonWebflowContent class="ButtonWebflow">{{ButtonWebflowContent}}</button></div>
        <a :src=LinkConect class="LinkConect">
            <div class="LinkAnimate">
                <div>{{LinkConect}}</div>
                <div class="LinkConectLine"></div>
            </div>
        </a>
    </div>
</template>


