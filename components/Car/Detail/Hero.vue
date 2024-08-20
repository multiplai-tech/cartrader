<script setup>
const props = defineProps({
	car: {
		type: Object,
	},
})
</script>

<template>
<div class="mt-10">
	<img :src="props.car.url" class="w-full" alt="" />
	<h1 class="mt-10 text-4xl">{{ props.car.name }}</h1>
	<div class="text-slate-500 flex text-lg mt-3 border-b pb-5 justify-between">
		<div class="flex">
			<p class="mr-2">{{ props.car.seats }} seats</p>
			<p class="mr-2">|</p>
			<p class="mr-2">{{ props.car.miles }} miles</p>
		</div>
		<div>
			<p class="font-bold text-2xl">${{ props.car.price }}</p>
		</div>
	</div>
</div>
</template>