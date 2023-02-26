<template>
    <div class="">
        <header class="shadow-md">
            <nav class="flex container mx-auto p-6 justify-between">
                <NuxtLink to="/" class="font-semibold text-xl">Ripkiii</NuxtLink>
                <ul class="flex gap-5">
                    <li><NuxtLink to="/">Home</NuxtLink></li>
                    <li><NuxtLink to="/about">About</NuxtLink></li>
                    <li><NuxtLink to="/products" class="bg-green-400 p-2 rounded-lg text-white">Products</NuxtLink></li>
                </ul>
            </nav>
        </header>
    </div>

    <div class="container mx-auto p-6">
        <slot />
    </div>
</template>

<style scoped>
    .router-link-exact-active {
        color: mediumseagreen;
    }
</style>