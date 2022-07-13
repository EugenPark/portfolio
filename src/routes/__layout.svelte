<script lang="ts">
	import Header from '$lib/header/Header.svelte';
	import Navbar from '$lib/navbar/Navbar.svelte';
	import '../app.css';

	let theme = 'light';
</script>

<!-- <Header /> -->

<Navbar bind:theme />

<main class="flex p-4 min-h-screen {theme === 'light' ? 'bg-linen' : 'bg-darkSienna'}">
	<div class="flex flex-col mx-auto max-w-2xl"><slot /></div>
</main>

<!-- <footer>
	<p>visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to learn SvelteKit</p>
</footer> -->
<style>
	main {
		margin: 0 auto;
		box-sizing: border-box;
	}

	footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 40px;
	}

	footer a {
		font-weight: bold;
	}

	@media (min-width: 480px) {
		footer {
			padding: 40px 0;
		}
	}
</style>
