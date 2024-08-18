<script setup>
useHead({
  titleTemplate: (titleChunk) => {
    return titleChunk ? `${titleChunk} - LoremIpsum` : 'LoremIpsum';
  }
})
</script>

<template>
<NuxtLayout>
	<NuxtPage />
</NuxtLayout>
</template>
