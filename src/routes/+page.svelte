<script>
	import Hero from '$lib/components/Hero.svelte';
</script>

<div class="">
	<Hero />

	<section class="u-container">
		<h2>What is KozoCSS?</h2>
		<p>
			KozoCSS is a copy-paste CSS framework that simplifies web development, giving you complete
			freedom to build your dream project without endless CSS overwrites.
		</p>
	</section>

	<section class="u-container">
		<h2>Quickstart</h2>
		<p>Begin by copying the foundation you need.</p>

		<ul>
			<li><a href="">reset.css</a></li>
			<li><a href="">typography.css</a></li>
			<li><a href="">spacing.css</a></li>
			<li><a href="">color.css</a></li>
		</ul>

		<p>Try more utilities using utils.css</p>

	</section>

	<section class="u-container">
		<h2>Inspiration</h2>

		<p>reset.css is based on Preflight from Tailwind CSS, a modern CSS reset.</p>

		<p>
			typography.css and spacing.css are responsive clamp-based values using <a
				href="https://utopia.fyi"
			>
				Utopia
			</a>
			to get universal text that adjust their sizes based on user's screens.
		</p>
	</section>

	<section class="u-container">
		<h2>Other Recommendation</h2>

		<p>⭐ Linting: eslint, <a href="https://perfectionist.dev/">perfectionist</a></p>
		<p>
			⭐ Learn B.E.M for a better CSS naming scheme: https://sparkbox.com/foundry/bem_by_example
		</p>
	</section>
</div>

<style>
	h2 {
		font-size: var(--step-4);
		font-weight: 500;
	}

	section {
		margin-bottom: var(--space-3xl);
		min-height: 40dvh;
	}

	p {
		max-width: 65ch;
		line-height: 1.6;
		font-size: var(--step-0);
	}
</style>
