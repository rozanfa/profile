<script lang="ts">
	import Terminal from '$lib/components/Terminal.svelte';
	import Projects from '$lib/sections/Projects.svelte';
	import Languages from '$lib/sections/Languages.svelte';
	import Tools from '$lib/sections/Tools.svelte';
	import Intro from '$lib/sections/Intro.svelte';
	import Contacts from '$lib/components/Contacts.svelte';
	import Works from '$lib/sections/Works.svelte';
</script>

<svelte:head>
	<title>Rozan Fadhil Al Hafidz</title>
	<meta
		name="description"
		content="Rozan Fadhil Al Hafidz's profile. A fourth-year Informatics Engineering student at Bandung Institute of Technology"
	/>
</svelte:head>

<section class="">
	<div class="w-full h-full">
		<Intro />
		<div class="bottom-section h-full pb-8">
			<div class="max-w-screen-xl mx-auto px-8">
				<div class="py-8">
					<Terminal />
				</div>
				<div class="py-8">
					<Works />
				</div>
				<div class="py-8">
					<Projects />
				</div>
				<div class="py-8">
					<Languages />
				</div>
				<div class="py-8">
					<Tools />
				</div>
				<div class="py-8">
					<Contacts />
				</div>
			</div>
		</div>
	</div>
</section>

<style lang="postcss">
	.bottom-section {
		background: rgb(143, 163, 255);
		background: linear-gradient(
			180deg,
			rgba(143, 163, 255, 1) 0%,
			rgba(143, 163, 255, 1) 0%,
			rgba(175, 175, 246, 1) 35%,
			rgba(250, 244, 187, 1) 100%
		);
	}
</style>
