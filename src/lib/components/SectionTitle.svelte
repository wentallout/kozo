<script>
	import LogoBlank from '$lib/components/art/LogoBlank.svelte';

	let { title = '' } = $props();
</script>

<a href="#{title.toLowerCase()}">
	<div id="#{title.toLowerCase()}" class="section-title">
		<LogoBlank />
		<h2>{title}</h2>
	</div>
</a>

<style>
	.section-title {
		display: flex;
		flex-direction: row;
		gap: var(--space-s);
		font-size: var(--step-4);
		align-items: center;
		margin-bottom: var(--space-m);
	}

	a {
		text-decoration: none;
	}

	h2 {
		margin-bottom: 0;
		background: var(--linearPrimarySecondary);

		color: transparent;
		background-clip: text;
	}
</style>
