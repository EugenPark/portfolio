<script context="module" lang="ts">
	export const prerender = true;
</script>

<script lang="ts">
	import WelcomeHeader from './home/welcomeHeader.svelte';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section><WelcomeHeader /></section>

<style>
</style>
