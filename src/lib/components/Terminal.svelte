<script lang="ts">
	import { onMount } from 'svelte';
	import { typewriter } from '$lib/utils/transitions';

	let shell: HTMLDivElement;
	let displayName = false;
	let displayIntro = false;
	let isTerminalVisible = false;

	onMount(() => {
		const observer = new IntersectionObserver((entries) => {
			entries.forEach((entry) => {
				isTerminalVisible = entry.isIntersecting;
			});
		});

		observer.observe(shell);
	});

	$: if (isTerminalVisible) {
		setTimeout(() => (displayName = true), 500);
	}
</script>

<section id="terminal">
	<div class="text-white w-full h-full terminal">
		<div class="h-[30px] w-full flex items-center justify-center text-sm">Terminal</div>
		<code
			class="flex flex-col text-left min-h-[500px] w-auto h-full justify-start items-start bg-black p-2 m-1 mt-0"
		>
			<div class="terminal-text">
				<div class="flex" bind:this={shell}>
					<div>sh#&nbsp;</div>
					{#if displayName}
						<div
							transition:typewriter={{ speed: 0.5 }}
							on:introend={() => setInterval(() => (displayIntro = true), 500)}
						>
							cat&nbsp;rozan
						</div>

						{#if !displayIntro}
							<div class="cursor"></div>
						{/if}
					{/if}
				</div>
				{#if displayIntro}
					<p class="mono">
						Hello, I am currently a seventh-semester university student pursuing a bachelor's degree
						in informatics engineering at Bandung Institute of Technology.
						<br />
						<br />
						I'm interested in web development, low-level programming, and deep learning
						<br />
						<br />
						I love to use Linux because it gives me flexibility to customize. I enjoy trying open source
						projects that available on Github to customize my operating system.
					</p>
					<br />
					<div class="flex">
						<div>sh#&nbsp;</div>
						<div class="cursor blinking"></div>
					</div>
				{/if}
			</div></code
		>
	</div>
</section>

<style lang="postcss">
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
	}

	h1 {
		width: 100%;
	}

	.welcome {
		display: block;
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
	}

	.welcome img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
	}

	.terminal {
		background-color: #777799bb;
	}

	.cursor {
		width: 2px;
		background-color: #f0f0f0;
		margin-left: 1px;
	}

	.blinking {
		animation: blink 1.2s step-start infinite;
	}

	@keyframes blink {
		0% {
			opacity: 1;
		}
		50% {
			opacity: 0;
		}
		100% {
			opacity: 1;
		}
	}
</style>
