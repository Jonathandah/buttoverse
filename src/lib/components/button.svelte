<script lang="ts">
	import { cn } from '$lib/utils/cn.js';
	import type { HTMLButtonAttributes } from 'svelte/elements';

	interface $$Props extends HTMLButtonAttributes {}

	const { class: klass, ...props }: $$Props = $$props;
</script>

<button class={cn('px-4 py-2', klass)}>
	<slot />
</button>
