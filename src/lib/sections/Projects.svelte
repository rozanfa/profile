<script lang="ts">
	import Chip from '$lib/components/Chip.svelte';
</script>

<section id="recent-projects">
	<h1 class="font-bold text-lg">Recent Projects</h1>
	<p class="text-center mb-4">Mainly consist of personal project and school project</p>
	<div class="grid grid-cols-2 md:grid-cols-4 gap-2">
		<Chip
			title="Dunia Material"
			description="A website for buying construction materials. Used NextJS, TailwindCSS, and MaterialUI. Implements internationalization to support multiple languages."
			span={2}
			bgColor="#ddbb40"
			time="Mar 2024"
		/>
		<Chip
			title="Jasmine Florist"
			description="A website for buying flowers and flower arrangements. Used PHP Laravel and TailwindCSS."
			span={2}
			bgColor="#eec3a7"
			link="https://jasmineflorist.co.id"
			time="Jan 2024"
		/>
		<Chip
			title="2-bit Pixel Art Generator"
			description="Generate 2-bit pixel art from given images. Using image processing techniques"
			span={2}
			bgColor="#ffa960"
			time="Jan 2024"
		/>
		<Chip
			title="Vehicle Detector"
			description="Detect vehicles from given images using machine learning and image processing techniques"
			span={2}
			bgColor="#ac88dd"
			link="https://github.com/rozanfa/IF4073-Tugas4-13520039-13520062-13520103"
			time="Nov 2023"
		/>
		<Chip
			title="SakuGwej: Personal Financial Tracking"
			description="Personal financial tracking that can create virtual bank accounts and record user’s incoming and outgoing
		money. Integrated to external mailer service using nodemailer"
			span={2}
			bgColor="#fbf930"
			time="May 2023"
			link="https://gitlab.informatika.org/if3250_2023_k01_05_sakugwej"
		/>
		<Chip
			title="Kud: Simple Version Control System"
			description="Simple Version Control System to records changes to set of files using bash script"
			span={2}
			bgColor="#eaefa0"
			time="Mar 2023"
			link="https://github.com/rozanfa/kud"
		/>
		<Chip
			title="Simple Restaurant Android App"
			description="Simple Restaurant Android App that allows user to order food and check restaurant's location. Also use CameraX to scan QR Code. Using Kotlin and Android Studio"
			span={2}
			bgColor="#c0d0d0"
			time="Feb 2023"
			link="https://gitlab.informatika.org/rozanfa/if3210-2023-android-pkr"
		/>
		<Chip
			title="Pekotify"
			description="Simple Spotify-like web application with an admin page that allows admins to put songs and users can listen to those
			songs. Used PHP, ReactJS, ExpressJS, SOAP, MySQL, and Docker"
			span={2}
			bgColor="#00b960"
			time="Nov 2022"
			link="https://gitlab.informatika.org/if3110-2022-k03-01-53/pekotify"
		/>
	</div>
</section>

<style lang="postcss">
</style>
