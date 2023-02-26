<template>
    <div>
        <!-- <h1 class="mb-4">This is a product page</h1> -->
        <div class="grid grid-cols-4 gap-5 gap-y-16">
            <div v-for="p in products">
                <ProductCard :product="p" />
            </div>
        </div>
    </div>
</template>

<script setup>
    definePageMeta({
        layout: 'products'
    })

    const { data: products } = await useFetch('https://fakestoreapi.com/products')
</script>

<style>

</style>