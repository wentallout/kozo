<script>
	import LogoBlank from '$lib/components/art/LogoBlank.svelte';

	let { title } = $props();
</script>

<div class="section-title">
	<LogoBlank />
	<h2>{title}</h2>
</div>

<style>
	.section-title {
		display: flex;
		flex-direction: row;
		gap: var(--space-s);
		font-size: var(--step-4);
		align-items: center;
		margin-bottom: var(--space-m);
	}

	h2 {
		margin-bottom: 0;
		background: var(--linearPrimarySecondary);

		color: transparent;
		background-clip: text;
	}
</style>
