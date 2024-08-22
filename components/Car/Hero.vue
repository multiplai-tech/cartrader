<script setup>
useHead({
  link: [{ rel: 'stylesheet', href: 'https://fonts.googleapis.com/css2?family=Barlow+Condensed:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap' }]
})
</script>

<template>
<div>
	<div class="relative z-1 flex items-center px-5 lg:px-20 h-[85vh] w-100 bg-no-repeat bg-cover bg-fixed bg-bottom bg-[url('https://images.unsplash.com/photo-1492144534655-ae79c964c9d7?q=80&w=2566&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D')] bg-[-550px_-100px] lg:bg-[center_-250px]">
		<div class="absolute top-0 left-0 w-full h-full bg-black opacity-50"></div>
		<div class="absolute text-white">
			<span class="flex justify-center lg:justify-normal lg:w-[650px]">
				<p class="text-6xl text-center lg:text-left lg:text-7xl font-bold">Lorem ipsum dolor sit amet consectetur.</p>
			</span>
			<p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat.</p>
		</div>
	</div>
	<div class="relative -mt-[5rem] w-full h-full flex justify-center items-center">
		<div class="flex items-center bg-white w-[90vw] lg:w-[70vw] rounded-lg shadow-md">
			<CarSearchBar />
		</div>
	</div>
	<div class="hidden md:block lg:block flex-col justify-center mb-20">
		<div class="flex flex-col text-center justify-center text-[#d3d3d3] text-[20rem] barlow-condensed-extrabold">
			<p>LOREM IPSUM</p>
		</div>
		<div class="-mt-72 md:-mt-[750px] lg:-mt-72 flex justify-center">
			<NuxtImg src="/img/car-1.png" class="aspect-auto h-[600px]" />
		</div>
	</div>
	<div class="grid mt-10 md:mt-36 lg:mt-10 lg:grid-cols-3 auto-rows-max gap-2 w-full h-auto px-2 lg:px-16">
		<div class="h-[300px] overflow-hidden rounded-xl lg:max-h-[70vh] lg:order-none lg:h-screen lg:col-span-2">
			<div class="transition-transform duration-300 transform scale-150 md:scale-110 lg:scale-110 bg-[center_100px] md:bg-[center_-40px] lg:bg-[center_0px] peer h-screen lg:h-screen bg-no-repeat bg-contain bg-[url('https://images.unsplash.com/photo-1592840062661-a5a7f78e2056?q=80&w=2532&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D')]"></div>
		</div>
		<div class="bg-[#1c1c1c] text-white rounded-xl flex flex-col w-100 lg:h-[70vh] p-5 lg:p-10">
			<p class="text-3xl mb-10 lg:text-5xl font-bold">Lorem ipsum dolor sit amet consectetur adipisicing.</p>
			<p class="text-1xl lg:text-2xl font-bold mt-auto">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quasi, quam! Dolor sit amet consectetur.</p>
		</div>
		<div class="order-2 lg:order-none bg-[#1c1c1c] text-white rounded-xl flex flex-col w-100 lg:h-[70vh] p-5 lg:p-10">
			<p class="text-3xl mb-10 lg:text-5xl font-bold">Lorem ipsum dolor sit amet consectetur adipisicing.</p>
			<p class="text-1xl lg:text-2xl font-bold mt-auto">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quasi, quam! Dolor sit amet consectetur.</p>
		</div>
		<div class="h-[300px] overflow-hidden rounded-xl order-1 lg:max-h-[70vh] lg:order-none lg:h-screen lg:col-span-2">
			<div class="transition-transform duration-300 transform scale-150 bg-[center_00px] md:bg-[center_-180px] lg:bg-[center_-200px] peer h-screen lg:h-screen bg-no-repeat bg-contain bg-[url('https://images.unsplash.com/photo-1537984822441-cff330075342?q=80&w=2574&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D')]"></div>
		</div>
	</div>
</div>
</template>

<style scoped>
.barlow-condensed-extrabold {
  font-family: "Barlow Condensed", sans-serif;
  font-weight: 800;
  font-style: normal;
}
</style>