<script>
	import '../app.css';
</script>

<main class="flex flex-col h-dvh  bg-gray-900 relative">
	<div aria-hidden class=" inset-1/2 absolute inset-x-0 w-16 h-16 rounded-full  bg-gradient-to-b from-pink-500 to-purple-600 blur-3xl mx-auto  opacity-75"/>
	<slot />
</main>
