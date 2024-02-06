<script lang="ts">
	import gmailLogo from '$lib/images/gmail.svg';
	import githubLogo from '$lib/images/github.svg';
	import instagramLogo from '$lib/images/instagram.svg';
	import discordLogo from '$lib/images/discord.svg';
	import linkedinLogo from '$lib/images/linkedin.svg';
</script>

<section id="contact-me">
	<div
		class="max-w-[450px] mx-auto text-white w-full h-full terminal text-black bg-green-100 p-4 rounded-lg border border-gray-900"
	>
		<h1 class="font-bold text-base md:text-lg md:mb-4 mb-2">Contact Me</h1>
		<div class="grid grid-cols-3 max-w-[350px] mx-auto text-xs md:text-base">
			<div class="flex items-center flex-1">
				<img src={linkedinLogo} alt="LinkedIn" class="w-4 h-4 mr-2" />
				<p>LinkedIn</p>
			</div>
			<p class="col-span-2 text-blue-700">
				:
				<a href="https://www.linkedin.com/in/rozan-fadhil-al-hafidz/"> Rozan Fadhil Al Hafidz </a>
			</p>
			<div class="flex items-center flex-1">
				<img src={gmailLogo} alt="Gmail" class="w-4 h-4 mr-2" />
				<p>Mail</p>
			</div>
			<p class="col-span-2">: rozanfadhilalhafidz@gmail.com</p>
			<div class="flex items-center">
				<img src={githubLogo} alt="Gmail" class="w-4 h-4 mr-2" />
				<p>Github</p>
			</div>
			<p class="col-span-2 text-blue-700">: <a href="https://github.com/rozanfa">rozanfa</a></p>
			<div class="flex items-center">
				<img src={discordLogo} alt="Gmail" class="w-4 h-4 mr-2" />
				<p>Discord:</p>
			</div>
			<p class="col-span-2">: bizeerr</p>
		</div>
	</div>
</section>

<style lang="postcss">
	h1,
	p {
		color: black;
	}
	a {
		color: #3366cc;
	}
</style>
