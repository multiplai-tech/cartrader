<script setup>
const route = useRoute()
const { data: car, refresh } = await useFetchCar(route.params.id)

const { toTitleCase } = useUtilities();

useHead({
	title: toTitleCase(route.params.name),
})

definePageMeta({
	layout: 'custom'
})
</script>

<template>
<div>
	<div>
		<CarDetailHero :car />
		<CarDetailAttributes :features="car.features" />
		<CarDetailDescription :description="car.description" />
		<CarDetailContact />
	</div>
</div>
</template>