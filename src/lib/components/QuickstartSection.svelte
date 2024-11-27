<script>
	import SectionTitle from '$lib/components/SectionTitle.svelte';
</script>

<section class="u-container">
	<SectionTitle title="Quickstart" />
	<p>Begin by copying these foundation that will help you build your design system.</p>

	<ul class="card">
		<li class="card__item">
			<a href="https://github.com/wentallout/kozo/blob/master/src/lib/styles/reset.css"
				>reset.css</a>
		</li>
		<li class="card__item">
			<a href="https://github.com/wentallout/kozo/blob/master/src/lib/styles/typography.css"
				>typography.css</a>
		</li>
		<li class="card__item">
			<a href="https://github.com/wentallout/kozo/blob/master/src/lib/styles/spacing.css"
				>spacing.css</a>
		</li>
		<li class="card__item">
			<a href="https://github.com/wentallout/kozo/blob/master/src/lib/styles/color.css"
				>color.css</a>
		</li>
	</ul>
</section>

<style>
	.card {
		display: grid;
		grid-template-columns: 1fr 1fr;
		grid-template-rows: 1fr 1fr;

		border-top: 1px solid var(--primary-500);
		border-left: 1px solid var(--primary-500);
		overflow: visible;
	}

	.card a {
		text-decoration: none;
		width: 100%;
		height: 100%;
		display: flex;
		justify-content: center;
		align-items: center;
		padding: var(--space-xs) var(--space-s);
		min-height: 10dvh;

		border-bottom: 1px solid var(--primary-500);
		border-right: 1px solid var(--primary-500);
	}

	.card a:hover {
		background-color: var(--primary-600);
		color: var(--background-100);
	}
</style>
