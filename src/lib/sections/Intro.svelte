<script lang="ts">
	import { onMount } from 'svelte';
	import { typewriter } from '$lib/utils/transitions';

	let displayDescription = false;

	onMount(() => {
		displayDescription = true;
	});

	function handleAnchorClick(event: any) {
		event.preventDefault();
		const link = event.currentTarget;
		const anchorId = new URL(link!.href).hash.replace('#', '');
		const anchor = document.getElementById(anchorId);
		window.scrollTo({
			top: anchor!.offsetTop,
			behavior: 'smooth'
		});
	}
</script>

<section class="main w-screen">
	<div class="intro-container min-w-screen">
		<h1 class="md:text-4xl text-3xl font-bold bg-blue-200 p-4 rounded-xl">
			Rozan Fadhil Al Hafidz
		</h1>
		<div class="flex md:flex-row flex-col text-center md:text-2xl gap-0 text-lg mt-4">
			<div>Interested in&nbsp;</div>
			{#if displayDescription}
				<div transition:typewriter={{ speed: 1.5 }}>
					web development, low-level programming, and deep learning
				</div>
			{/if}
		</div>
		<div
			class="flex gap-4 text-indigo-600 pt-2 md:flex-row flex-col text-center mt-2 border-t border-indigo-500"
		>
			<a href="#terminal" on:click={handleAnchorClick}>About Me</a>
			<a href="#recent-projects" on:click={handleAnchorClick}>Recent Projects</a>
			<a href="#languages" on:click={handleAnchorClick}>Programming Languages</a>
			<a href="#tools" on:click={handleAnchorClick}>Tools</a>
			<a href="#contact-me" on:click={handleAnchorClick}>Contact Me</a>
		</div>
	</div>
</section>

<style lang="postcss">
	.intro-container {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		height: 100vh;
		padding: 0px 4px;
		width: 100vw;
	}

	.main {
		background-color: #8fa3ff;
	}
</style>
