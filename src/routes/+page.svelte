<script>
	import Button from '$lib/components/button.svelte';
</script>

<div class="m-auto">
	<div class="flex flex-col gap-4">
		<Button
			class="border border-gray-900 bg-gray-200 py-0 text-gray-900 hover:bg-gray-300/80 active:border-gray-500 active:bg-gray-100"
			>Default
		</Button>

		<Button class="rounded bg-indigo-600 text-white shadow hover:bg-indigo-600/90">Modern</Button>

		<Button
			class="dark:border-input rounded border border-indigo-300 text-indigo-700 hover:bg-indigo-50 hover:text-indigo-800"
		>
			Modern outline
		</Button>

		<Button class="border border-gray-400 text-gray-700 hover:bg-gray-50 hover:text-gray-800">
			Noir outline
		</Button>

		<Button
			class="rounded bg-green-600 text-white shadow transition hover:scale-125 hover:bg-green-600/90 active:scale-110"
		>
			Scaler
		</Button>

		<Button
			class="rounded bg-gradient-to-r from-green-400 to-yellow-300 text-gray-900 hover:from-green-400/90 hover:to-yellow-300/90 "
		>
			Gradient
		</Button>

		<Button class="rounded bg-blue-600 text-white transition hover:rotate-180 hover:bg-blue-600/90">
			Spinnerui
		</Button>
	</div>
</div>
