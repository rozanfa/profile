<script>
	import Header from './Header.svelte';
	import './styles.css';
	import '../app.css';
</script>

<div class="app">
	<!-- <Header /> -->

	<main>
		<slot />
	</main>

	<footer>
		<p>Created by Rozan Fadhil Al Hafidz using Svelte Framework</p>
		<a class="ext" href="https://simpleicons.org/" title="Simple Icons">Icons by Simple Icons</a>
	</footer>
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		width: 100%;
		margin: 0 auto;
		box-sizing: border-box;
	}

	footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 12px;
		background-color: #000;
		color: #fff;
		font-size: 12px;
	}

	.ext {
		font-size: 10px;
	}

	@media (min-width: 480px) {
		footer {
			padding: 12px 0;
		}
	}
</style>
