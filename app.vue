<template>
<div>
	<!-- NAVBAR -->
	<header class="sticky top-0 z-50 flex justify-between items-center space-x-1 border-b bg-white p-4 shadow-md">
		<a class="text-3xl font-mono space-x-6" href="#">Cartrader</a>
	</header>
	<!-- NAVBAR -->
	
	<!-- CARS PAGE -->
	<div class="mx-auto mt-4 max-w-7xl space-y-4 px-4 xs:px-8 sm:px-10 lg:px-16 pb-16 w-3/5">
		<div class="mt-32 flex">
			<!-- CAR SIDE BAR -->
			<div class="shadow border w-64 mr-10 z-30 h-[190px]">
				<div class="p-5 flex justify-between relative cursor-pointer border-b">
					<h3>Location</h3>
					<h3 class="text-blue-400 capitalize">Cavite</h3>
					<!-- <div class="absolute border shadow left-56 p-5 top-1 -m-1 bg-white">
						<input type="text" class="border p-1 rounded" />
						<button class="bg-blue-400 w-full mt-2 rounded text-white p-1">Apply</button>
					</div> -->
				</div>

				<div class="p-5 flex justify-between relative cursor-pointer border-b">
					<h3>Make</h3>
					<h3 class="text-blue-400 capitalize">Toyota</h3>
				</div>
				
				<div class="p-5 flex justify-between relative cursor-pointer border-b">
					<h3>Price</h3>
					<h3 class="text-blue-400 capitalize">Any</h3>
				</div>
			</div>
			<!-- CAR SIDE BAR -->
			
			<!-- CAR CARDS -->
			<div class="w-full">
				<!-- CAR CARD -->
				<div class="shadow border w-full overflow-hidden mb-5 cursor-pointer h-[200px]">
					<div class="flex h-full">
						<img src="https://carconfigurator.ferrari.com/rt-assets/data/cars/812competizione-a/ui/splashpage.jpg" class="w-[300px] h-full bg-fixed" />
						<div class="p-4 flex flex-col">
							<div>
								<h1 class="text-2xl text-blue-700">Volvo XC40</h1>
								<p class="text-gray-700">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
							</div>
							<h1 class="mt-auto text-xl">$3,900.55</h1>
						</div>
					</div>
				</div>
				<!-- CAR CARD -->
			</div>
			<!-- CAR CARDS -->
		</div>
	</div>
	<!-- CARS PAGE -->
</div>
</template>
