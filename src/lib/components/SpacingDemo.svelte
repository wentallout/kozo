<script>
	let spaces = ['3xs', '2xs', 'xs', 's', 'm', 'l', 'xl', '2xl', '3xl'];
</script>

<section>
	<h3>Spacing</h3>

	<div class="demo">
		{#each spaces as space}
			<div class="space space--{space}">
				<div class="circle"></div>
				<div class="circle"></div>
			</div>
		{/each}
	</div>
</section>

<style>
	.circle {
		aspect-ratio: 1;
		width: 16px;
		height: 16px;
		background-color: var(--primary-500);
		border-radius: 100%;
		margin-bottom: var(--space-s);
	}

	.space {
		display: flex;
	}

	.space--3xs {
		gap: var(--space-3xs);
	}

	.space--2xs {
		gap: var(--space-2xs);
	}

	.space--xs {
		gap: var(--space-xs);
	}

	.space--s {
		gap: var(--space-s);
	}

	.space--m {
		gap: var(--space-m);
	}

	.space--l {
		gap: var(--space-l);
	}

	.space--xl {
		gap: var(--space-xl);
	}

	.space--2xl {
		gap: var(--space-2xl);
	}

	.space--3xl {
		gap: var(--space-3xl);
	}
</style>
