<script setup>
const route = useRoute()

const { data: cars, refresh } = await useFetchCars(route.params.city, {
	minPrice: route.query.minPrice,
	maxPrice: route.query.maxPrice,
	make: route.query.make
})

watch(
	() => route.query,
	() => {
		window.location.reload(true)
	}
)
</script>

<template>
<div>
	<CarCards v-if="cars.length" :cars="cars"/>
	<h1 v-else class="text-red-400">No Cars Found</h1>
</div>
</template>