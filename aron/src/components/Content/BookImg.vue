<script setup lang="ts">
import part2 from '../styles/part2.module.css'
const BookImage = "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61bb27f9cecada1a656a3b3b_photo-3.jpg"
const ColorImage = "https://assets.website-files.com/61b88a38b30a977e957e8ca7/61bb298c9a00f35962080d9f_photo-4.jpg"

</script>
<template>
    <img :src=BookImage :class="part2.BookImage"/>
    <img :src=ColorImage :class="part2.ColorImage"/>
</template>
