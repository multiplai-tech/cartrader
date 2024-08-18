<script setup>
const route = useRoute()
useHead({
	title: `${route.params.make ? route.params.make : 'Cars'} in ${route.params.city.toLocaleUpperCase()}`
})

definePageMeta({
	layout: 'custom'
})
</script>

<template>
<div class="mt-32 flex">
	<CarSideBar />
	<NuxtPage />
</div>
</template>