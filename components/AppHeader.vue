<script setup>
const route = useRoute()
</script>

<template>
<!-- <header class="fixed w-full top-0 z-50 flex justify-between items-center space-x-1 p-4 px-20" :class="route.path === '/' ? 'backdrop-blur-md' : 'bg-[#0f151b]'"> -->
<header class="fixed w-full top-0 z-50 flex justify-between items-center space-x-1 p-4 px-20" :class="route.path === '/' ? '' : 'bg-[#0f151b]'">
	<NuxtLink class="text-2xl text-white font-medium space-x-6" to="/">LoremIpsum</NuxtLink>
</header>
</template>