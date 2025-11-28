<template>
	<UFooter>
		<template #left>
			<p class="text-muted text-sm">
				Copyright © {{ new Date().getFullYear() }}
			</p>
		</template>

		<template #right>
			<UButton
				icon="i-simple-icons-facebook"
				color="neutral"
				variant="ghost"
				to="https://fb.me/anhdaijka"
				target="_blank"
				aria-label="Facebook"
			/>
			<UButton
				icon="i-simple-icons-instagram"
				color="neutral"
				variant="ghost"
				to="https://instagram.com/anhdaijka"
				target="_blank"
				aria-label="Instagram"
			/>
			<UButton
				icon="i-simple-icons-github"
				color="neutral"
				variant="ghost"
				to="https://github.com/anhdaijka"
				target="_blank"
				aria-label="GitHub"
			/>
		</template>
	</UFooter>
</template>
