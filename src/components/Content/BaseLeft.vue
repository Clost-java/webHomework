<script setup>
const props = defineProps(['images'])
</script>

<template>
<div class="imgbox left">
    <img :src="images.url" alt="">
</div>
</template>

<style scoped>

img{
    width: 254px;
    height: 614px;
}

</style>