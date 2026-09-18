<script lang="ts">
	import javascriptLogo from '$lib/images/javascript.svg';
	import typescriptLogo from '$lib/images/typescript.svg';
	import pythonLogo from '$lib/images/python.svg';
	import dartLogo from '$lib/images/dart.svg';
	import cLogo from '$lib/images/c.svg';
	import csharpLogo from '$lib/images/csharp.svg';
	import cplusplusLogo from '$lib/images/cplusplus.svg';
	import kotlinLogo from '$lib/images/kotlin.svg';
	import gnubashLogo from '$lib/images/gnubash.svg';
	import phpLogo from '$lib/images/php.svg';
	import golangLogo from '$lib/images/go.svg';
	import Chip from '$lib/components/Chip.svelte';
	import { onMount } from 'svelte';

	let displaySectionTitle = false;

	onMount(() => {
		displaySectionTitle = true;
	});
</script>

<section id="languages">
	{#if displaySectionTitle}
		<h2 class="font-bold text-lg mb-4">Some Programming Languages I Have Used</h2>
	{/if}
	<div class="grid grid-cols-2 md:grid-cols-4 gap-2">
		<Chip
			logos={[javascriptLogo, typescriptLogo]}
			title="JavaScript & TypeScript"
			description="used for developing web apps and backend projects using Node.js"
			span={2}
			bgColor="#f7df1e"
		/>
		<Chip
			logo={pythonLogo}
			title="Python"
			description="used for data science, machine learning, and simple backend projects"
			span={2}
			bgColor="#3776ab"
		/>
		<Chip
			logo={golangLogo}
			title="Go"
			description="used for developing backend projects"
			span={2}
			bgColor="#00b4ab"
		/>
		<Chip
			logo={phpLogo}
			title="PHP"
			description="used for developing monolithic web apps"
			span={2}
			bgColor="#239120"
		/>
		<Chip
			logo={dartLogo}
			title="Dart"
			description="used for developing multi-platform apps using Flutter"
			span={2}
			bgColor="#0175C2"
		/>
		<Chip
			logo={kotlinLogo}
			title="Kotlin"
			description="used for developing Android apps"
			span={2}
			bgColor="#0095d5"
		/>
		<Chip
			logo={gnubashLogo}
			title="Bash"
			description="used for automating tasks in Linux"
			span={2}
			bgColor="#4eaa25"
		/>
		<Chip
			logo={cLogo}
			title="C"
			description="used for developing low-level programs (e.g. operating system)"
			span={2}
			bgColor="#a8b9cc"
		/>
		<Chip
			logo={cplusplusLogo}
			title="C++"
			description="used for competitive programming and developing low-level programs"
			span={2}
			bgColor="#00599c"
		/>
		<Chip
			logo={csharpLogo}
			title="C#"
			description="used for developing desktop apps using .NET and games using Unity"
			span={2}
			bgColor="#239120"
		/>
	</div>
</section>

<style lang="postcss">
</style>
