<script context="module" lang="ts">
	import Navbar from '$lib/navbar/Navbar.svelte';
	export const prerender = true;
</script>

<Navbar />

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<style>
</style>
