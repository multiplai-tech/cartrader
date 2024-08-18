<script setup>
const city = ref('')
const cityError = ref(false)

const handleSearch = () => {
	if (!city.value) {
		return cityError.value = true
	}
	navigateTo(`/city/${city.value}/car`)
}
</script>

<template>
<div class="flex flex-col lg:flex-row gap-5 justify-between items-center w-full p-10">
	<input
		v-model="city"
		@keyup.enter="handleSearch"
		type="text"
		class="bg-[#f5f6fa] w-full rounded-md p-5 focus:outline-none"
		:class="cityError ? 'border border-red-500 rounded-tr-none rounded-br-none' : ''"
		placeholder="Search by City">
	<input
		v-model="city"
		@keyup.enter="handleSearch"
		type="text"
		class="bg-[#f5f6fa] w-full rounded-md p-5 focus:outline-none"
		:class="cityError ? 'border border-red-500 rounded-tr-none rounded-br-none' : ''"
		placeholder="From">
	<input
		v-model="city"
		@keyup.enter="handleSearch"
		type="text"
		class="bg-[#f5f6fa] w-full rounded-md p-5 focus:outline-none"
		:class="cityError ? 'border border-red-500 rounded-tr-none rounded-br-none' : ''"
		placeholder="To">
	<button class="w-full lg:w-2/5 py-5 px-20 rounded-md bg-[#0f151b] text-white hover:bg-[#19222a] text-center" @click="handleSearch">Search</button>
</div>
</template>