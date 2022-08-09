<script lang="ts">
	import '../app.css';
</script>

<div class="container mx-auto flex flex-col h-screen">
	<header class="flex justify-evenly py-4 font-bold text-2xl">
		<nav class="item">
			<a href="/">Home</a>
		</nav>
		<nav class="item">
			<a href="/playlist">Playlist</a>
		</nav>
		<nav class="item"><a href="/about"> About</a></nav>
	</header>
	<main class="flex flex-col justify-center items-center grow">
		<slot />
	</main>
	<footer class="self-center py-2">Svelte Kit</footer>
</div>

<style>
	.item {
		@apply hover:text-blue-300;
	}
</style>
