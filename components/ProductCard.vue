<template>
    <div class="card text-center">
        <img :src="product.image" alt="prod thumb" class="thumb">
        <h2 class="text-xl font-bold mx-4 mt-5 truncate">{{product.title}}</h2>
        <NuxtLink :to="`/products/${product.id}`">
            <p class="btn">View details</p>
        </NuxtLink>
    </div>
</template>

<script setup>
    const { product } = defineProps(['product'])
</script>

<style scoped>
    .thumb {
        max-width: 70%;
        max-height: 120px;
        margin: 0px auto;
    }
</style>