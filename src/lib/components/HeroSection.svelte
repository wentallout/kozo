<script>
	import Logo from './art/Logo.svelte';
</script>

<section class="hero">
	<div class="u-container">
		<h1 class="hero__title">
			<Logo />
			KozoCSS
		</h1>
		<p class="hero__text">True vanilla copy-paste CSS framework</p>
	</div>
</section>

<style>
	.hero {
		min-height: 40dvh;
		background-color: black;
		color: white;
		width: 100%;
		margin-bottom: var(--space-xl);
		position: relative;
	}

	.hero::before {
		background: url('/images/bg.webp');
		content: '';
		object-fit: cover;
		opacity: 0.3;
		pointer-events: none;
		width: 100%;
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		z-index: 3;
	}

	.hero__title {
		font-size: var(--step-5);
		font-weight: 500;
		display: flex;
		flex-direction: row;
		align-items: center;
		gap: var(--space-m);
	}

	.hero__text {
		font-size: var(--step-2);
	}
</style>
