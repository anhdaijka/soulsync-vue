<script setup lang="ts">
const links = ref([
	{
		label: "Get started",
		to: "/docs/getting-started",
		icon: "i-lucide-square-play",
	},
	{
		label: "Learn more",
		to: "/docs/getting-started/theme/design-system",
		color: "neutral" as const,
		variant: "subtle",
		trailingIcon: "i-lucide-arrow-right",
	},
]);
</script>

<template>
	<UPageHero
		title="Soul Sync"
		description="Discover the world of smart dating with our exact matching system, which will help you find your ideal mate based on your zodiac sign, numerology, location, and interests.  Connect quickly, chat promptly, and keep your personal information strictly confidential.  No more waiting in vain; your love is only a click away!"
		headline="New release"
	>
		<div class="flex mx-auto md:flex-row items-center gap-2">
			<UButton
				icon="i-lucide:arrow-up-right"
				size="xl"
				color="primary"
				variant="solid"
				to="/auth"
				>Get Started</UButton
			>
			<UButton
				icon="i-lucide-rocket"
				size="xl"
				variant="outline"
				to="https://github.com/anhdaijka/soulsync-vue"
				target="_blank"
				>Release</UButton
			>
		</div>
	</UPageHero>
</template>
