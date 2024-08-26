<script setup>
const props = defineProps({
	cars: {
		type: Array
	}
})

const favorite = useLocalStorage("favorite", {});

const handleFavorite = (id) => {
	if (id in favorite.value) {
		delete favorite.value[id]
	} else {
		favorite.value = {
			...favorite.value,
			[id]: true
		}
	}
}
</script>

<template>
<div>
	<div class="w-full">
		<CarCard v-for="car in props.cars" :key="car.id" :car="car" :favored="car.id in favorite" @favor="handleFavorite"/>
	</div>
</div>
</template>