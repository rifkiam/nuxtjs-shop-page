<template>
    <div>
        <header class="shadow-md ">
            <nav class="container mx-auto p-6">
                <NuxtLink to="/" class="font-semibold text-xl">Ripkiii Shop</NuxtLink>
            </nav>
        </header>
    </div>

    <div class="container mx-auto p-6">
        <slot />
    </div>

    <footer class="container mx-auto p-6 flex justify-between border-t-2">
        <ul class="flex gap-5">
            <li><NuxtLink to="/">Home</NuxtLink></li>
            <li><NuxtLink to="/about">About</NuxtLink></li>
            <li><NuxtLink to="/products" class="bg-green-400 p-2 rounded-lg text-white">Products</NuxtLink></li>
        </ul>
    </footer>
</template>