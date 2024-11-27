<script>
	import { onMount } from 'svelte';

	let fontSize = [];

	onMount(() => {
		const elements = document.querySelectorAll(
			'.scale-0, .scale-1, .scale-2, .scale-3, .scale-4, .scale-5'
		);
		elements.forEach((element, index) => {
			const observer = new ResizeObserver(() => {
				const style = getComputedStyle(element);
				fontSize[index] = style.fontSize;
			});
			observer.observe(element);
		});
	});
</script>

<div class="demo">
	<div class="scale-0 nowrap">The quick brown fox jumps over the lazy dog</div>
	<div class="scale-1 nowrap">The quick brown fox jumps over the lazy dog</div>
	<div class="scale-2 nowrap">The quick brown fox jumps over the lazy dog</div>
	<div class="scale-3 nowrap">The quick brown fox jumps over the lazy dog</div>
	<div class="scale-4 nowrap">The quick brown fox jumps over the lazy dog</div>
	<div class="scale-5 nowrap">The quick brown fox jumps over the lazy dog</div>
</div>
<div>
	Font sizes:
	{#each fontSize as size, index}
		<div class="">
			--step-{index}: {size}
		</div>
	{/each}
</div>

<style>
	.scale-0 {
		font-size: var(--step-0);
	}

	.scale-1 {
		font-size: var(--step-1);
	}

	.scale-2 {
		font-size: var(--step-2);
	}

	.scale-3 {
		font-size: var(--step-3);
	}

	.scale-4 {
		font-size: var(--step-4);
	}

	.scale-5 {
		font-size: var(--step-5);
	}
</style>
