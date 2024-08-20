<script setup>
const props = defineProps({
	car: {
		type: Object
	}
})
</script>

<template>
<div class="shadow border w-full overflow-hidden mb-5 cursor-pointer h-[200px]" @click="navigateTo(`/car/${props.car.name}-${props.car.id}`)">
	<div class="flex h-full">
		<img :src="props.car.url" :alt="props.car.name" class="w-[300px] h-full" />
		<div class="p-4 flex flex-col">
			<div>
				<h1 class="text-2xl text-blue-700">{{ props.car.name }}</h1>
				<p class="text-gray-700">
					{{ props.car.description }}
				</p>
			</div>
			<h1 class="mt-auto text-xl">${{ props.car.price }}</h1>
		</div>
	</div>
</div>
</template>