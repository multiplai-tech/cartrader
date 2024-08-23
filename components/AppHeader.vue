<script setup>
const supabase = useSupabaseClient()
const route = useRoute()
const user = useSupabaseUser()

const signOut = async () => {
  	const { error } = await supabase.auth.signOut()
  	if (error) console.log(error)

	navigateTo('/')
}
</script>

<template>
<header class="fixed text-white w-full top-0 z-50 flex justify-between items-center space-x-1 p-4 px-20" :class="route.path === '/' ? '' : 'bg-[#0f151b]'">
	<NuxtLink class="text-2xl text-white font-medium space-x-6" to="/">LoremIpsum</NuxtLink>
	<div v-if="user" class="flex">
		<NuxtLink class="mr-5" to="/profile/listings">Profile</NuxtLink>
		<p class="cursor-pointer" @click="signOut">Logout</p>
	</div>
	<NuxtLink v-else to="/login">Login</NuxtLink>
</header>
</template>