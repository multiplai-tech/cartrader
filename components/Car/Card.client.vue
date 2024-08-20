<script setup>
import heartFilled from '@/assets/icons/heart/filled.png'
import heartOutline from '@/assets/icons/heart/outline.png'

const props = defineProps({
	car: Object,
	favored: Boolean,
})

const emit = defineEmits(['favor'])
</script>

<template>
<div class="relative shadow border w-full overflow-hidden mb-5 cursor-pointer h-[200px]">
	<img :src="props.favored ? heartFilled : heartOutline" class="absolute w-7 right-5 top-2 z-20" @click="emit('favor', car.id)" />
	<div class="flex h-full" @click="navigateTo(`/car/${props.car.name}-${props.car.id}`)">
		<NuxtImg :src="props.car.url" :alt="props.car.name" class="w-[300px] h-full" />
		<div class="p-4 flex flex-col">
			<div>
				<h1 class="text-2xl text-blue-700">{{ props.car.name }}</h1>
				<p class="text-gray-700">
					{{ props.car.description }}
				</p>
			</div>
			<h1 class="mt-auto text-xl">${{ props.car.price }} hehe</h1>
		</div>
	</div>
</div>
</template>