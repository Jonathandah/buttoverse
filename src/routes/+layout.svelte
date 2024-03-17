<script>
	import '../app.css';
</script>

<main class="relative flex flex-col h-dvh">
	<div aria-hidden class="absolute inset-x-0 w-16 h-16 mx-auto rounded-full opacity-75 inset-1/3 bg-gradient-to-b from-pink-500 to-purple-600 blur-3xl"/>
	<slot />
</main>
