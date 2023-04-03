<script setup lang="ts">
const BookImage = "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61bb27f9cecada1a656a3b3b_photo-3.jpg"
const ColorImage = "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61bb298c9a00f35962080d9f_photo-4.jpg"
import '../styles/part2.css'
</script>
<template>
    <img :src=BookImage class="BookImage"/>
    <img :src=ColorImage class="ColorImage"/>
</template>
