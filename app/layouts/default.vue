<template>
	<Header />
	<UContainer class="min-h-screen w-full">
		<slot />
	</UContainer>
	<Footer />
</template>

<script setup>
import Header from "../components/ui/Header.vue";
import Footer from "../components/ui/Footer.vue";
</script>
