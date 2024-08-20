<script setup>
const route = useRoute()
const { cars } = useCars();
const { toTitleCase } = useUtilities();

useHead({
	title: toTitleCase(route.params.name),
})

const car = computed(() => {
	return cars.find((car) => {
		return car.id === parseInt(route.params.id)
	})
})

if(!car.value) {
	throw createError({
		statusCode: 500,
		statusMessage: `Car with ID of ${ route.params.id } does not exist`
	})
}

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