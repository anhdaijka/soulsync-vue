<script setup lang="ts">
import type { NavigationMenuItem } from "@nuxt/ui";

const route = useRoute();

const items = computed<NavigationMenuItem[]>(() => [
	{
		label: "Home",
		to: "/",
		icon: "i-lucide-home",
		active: route.path === "/",
	},
	{
		label: "About",
		to: "/docs/about",
		icon: "i-lucide-info",
		active: route.path.startsWith("/docs/about"),
	},
	{
		label: "Repository",
		icon: "i-lucide-rocket",
		to: "https://github.com/anhdaijka/soulsync-vue",
		target: "_blank",
	},
	{
		label: "Author",
		icon: "i-lucide-user",
		to: "https://anhdaijka.vercel.app",
		target: "_blank",
	},
]);
</script>

<template>
	<UHeader mode="drawer">
		<template #title>
			<p class="font-bold">Soul <span class="text-primary">Sync</span></p>
		</template>

		<UNavigationMenu :items="items" />

		<template #right>
			<UColorModeButton />

			<UTooltip text="Login" :kbds="['meta', 'A']">
				<UButton
					color="neutral"
					variant="ghost"
					to="/auth"
					icon="i-lucide:circle-user-round"
					aria-label="Authenticate"
				/>
			</UTooltip>
		</template>

		<template #body>
			<UNavigationMenu :items="items" orientation="vertical" class="-mx-2.5" />
		</template>
	</UHeader>
</template>
