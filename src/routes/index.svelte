<script context="module" lang="ts">
	import Navbar from '$lib/navbar/Navbar.svelte';
	import Bio from '$lib/home/bio/Bio.svelte';
	export const prerender = true;
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<div class="flex"><Bio /></div>

<style>
</style>
