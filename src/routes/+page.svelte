<script>
	import Button from '$lib/components/button.svelte';
	import { cn } from '$lib/utils/cn.ts';
	import { animate, glide } from 'motion';
	import { onMount } from 'svelte';
	const CARD_OFFSET = 10;
	const SCALE_FACTOR = 0.06;

	const buttonList = [
		{
			text: 'Default',
			class:
				'border border-gray-900 bg-gray-200 py-0 text-gray-900 hover:bg-gray-300/80 active:border-gray-500 active:bg-gray-100'
		},
		{
			text: 'Modern',
			class: 'rounded bg-indigo-600 text-white shadow hover:bg-indigo-600/90'
		},
		{
			text: 'Modern outline',
			class:
				'dark:border-input rounded border border-indigo-300 text-indigo-700 hover:bg-indigo-50 hover:text-indigo-800'
		},
		{
			text: 'Noir outline',
			class: 'border border-gray-400 text-gray-700 hover:bg-gray-50 hover:text-gray-800'
		},
		{
			text: 'Scaler',
			class:
				'rounded bg-green-600 text-white shadow transition hover:scale-125 hover:bg-green-600/90 active:scale-110'
		},
		{
			text: 'Gradient',
			class:
				'rounded bg-gradient-to-r from-green-400 to-yellow-300 text-gray-900 hover:from-green-400/90 hover:to-yellow-300/90'
		},
		{
			text: 'Spinnerui',
			class: 'rounded bg-blue-600 text-white transition hover:rotate-180 hover:bg-blue-600/90'
		}
	];

	onMount(() => {
		// animate(
		// 	'#carousel',
		// 	{ y: 0,

		// 	},
		// 	{
		// 		easing: glide({ velocity: -500 }),
		// 		repeat: Infinity
		// 	}
		// );

		buttonList.forEach((_, index) => {
			// animate(
			// 	'#button-' + index,
			// 	{
			// 		top: index * -CARD_OFFSET,
			// 		scale: 1 - index * SCALE_FACTOR, // decrease scale for cards that are behind
			// 		zIndex: buttonList.length - index //  decrease z-index for the cards that are behind
			// 	},
			// 	{
			// 		// easing: glide({ velocity: -500 }),
			// 		repeat: Infinity
			// 	}
			// );
		});
	});
</script>

<div class="mx-auto mt-auto">
	<div id="carousel" class="inline-flex flex-col gap-4">
		{#each buttonList as button, index}
			<Button id={`button-${index}`} class={cn('', button.class)}>{button.text}</Button>
		{/each}
	</div>
</div>
