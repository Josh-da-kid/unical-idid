<script lang="ts">
	import 'carbon-components-svelte/css/all.css';
	import favicon from '$lib/assets/favicon.svg';
	import '../app.css';
	import Footer from '$lib/components/Footer.svelte';
	import Navbar from '$lib/components/Navbar.svelte';
	let { children } = $props();
</script>

<Navbar />

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children()}

<Footer />
