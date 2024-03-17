<script>
	import '../app.css';
</script>

<main class="relative flex h-dvh flex-col">
	<div
		aria-hidden
		class="absolute inset-1/3 inset-x-0 mx-auto h-16 w-16 rounded-full bg-gradient-to-b from-pink-500 to-purple-600 opacity-75 blur-3xl"
	/>
	<slot />
</main>
