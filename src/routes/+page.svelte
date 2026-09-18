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
	<title>Rozan Fadhil Al Hafidz | Fullstack Developer & Software Engineer</title>
	<meta
		name="description"
		content="Personal portfolio of Rozan Fadhil Al Hafidz, a Fullstack Developer and Informatics Engineering student at Bandung Institute of Technology (ITB) specializing in web development, low-level programming, and deep learning."
	/>
	<meta
		name="keywords"
		content="Rozan Fadhil Al Hafidz, Rozan Fadhil, Rozan, Software Engineer, Fullstack Developer, Informatics Engineering, Bandung Institute of Technology, ITB, Svelte, Next.js, Python, Go, Portfolio"
	/>
	<meta name="robots" content="index, follow" />
	<link rel="canonical" href="https://rozanfa.codes/" />

	<!-- Open Graph / Facebook -->
	<meta property="og:type" content="website" />
	<meta property="og:site_name" content="Rozan Fadhil Al Hafidz" />
	<meta property="og:url" content="https://rozanfa.codes/" />
	<meta property="og:title" content="Rozan Fadhil Al Hafidz | Fullstack Developer & Software Engineer" />
	<meta
		property="og:description"
		content="Personal portfolio of Rozan Fadhil Al Hafidz, a Fullstack Developer and Informatics Engineering student at ITB specializing in web development, low-level programming, and deep learning."
	/>
	<meta property="og:image" content="https://rozanfa.codes/favicon.png" />
	<meta property="og:locale" content="en_US" />

	<!-- Twitter -->
	<meta name="twitter:card" content="summary" />
	<meta name="twitter:url" content="https://rozanfa.codes/" />
	<meta name="twitter:title" content="Rozan Fadhil Al Hafidz | Fullstack Developer & Software Engineer" />
	<meta
		name="twitter:description"
		content="Personal portfolio of Rozan Fadhil Al Hafidz, a Fullstack Developer and Informatics Engineering student at ITB."
	/>
	<meta name="twitter:image" content="https://rozanfa.codes/favicon.png" />

	<!-- JSON-LD Structured Data for Search Engines -->
	{@html `<script type="application/ld+json">
	{
		"@context": "https://schema.org",
		"@graph": [
			{
				"@type": "Person",
				"@id": "https://rozanfa.codes/#person",
				"name": "Rozan Fadhil Al Hafidz",
				"alternateName": ["Rozan Fadhil", "rozanfa"],
				"url": "https://rozanfa.codes/",
				"image": "https://rozanfa.codes/favicon.png",
				"jobTitle": "Fullstack Developer & Software Engineer",
				"alumniOf": {
					"@type": "EducationalOrganization",
					"name": "Bandung Institute of Technology",
					"sameAs": "https://www.itb.ac.id"
				},
				"sameAs": [
					"https://github.com/rozanfa",
					"https://www.linkedin.com/in/rozan-fadhil-al-hafidz/"
				],
				"knowsAbout": [
					"Web Development",
					"Software Engineering",
					"Low-level Programming",
					"Deep Learning",
					"JavaScript",
					"TypeScript",
					"Python",
					"Go",
					"Svelte",
					"Next.js"
				]
			},
			{
				"@type": "WebSite",
				"@id": "https://rozanfa.codes/#website",
				"url": "https://rozanfa.codes/",
				"name": "Rozan Fadhil Al Hafidz Portfolio",
				"description": "Portfolio of Rozan Fadhil Al Hafidz",
				"publisher": {
					"@id": "https://rozanfa.codes/#person"
				},
				"inLanguage": "en-US"
			}
		]
	}
	</script>`}
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
