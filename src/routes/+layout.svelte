<script>
	import Footer from '$lib/components/Footer.svelte';
	import NavBar from '$lib/components/NavBar.svelte';

	import '$lib/styles/global.css';

	let { children } = $props();
	// Supports weights 300-900
	import '@fontsource-variable/rubik';
</script>

<NavBar />
<main>
	{@render children()}
</main>
<Footer />

<style>
	main {
		min-height: 100dvh;
	}
</style>
