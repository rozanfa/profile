<script lang="ts">
	import Chip from '$lib/components/Chip.svelte';
</script>

<section id="carier-history">
	<h1 class="font-bold text-lg mb-4">Carier History</h1>
	<div class="grid grid-cols-2 md:grid-cols-4 gap-2">
		<Chip
			title="Fullstack Developer Intern - GlobalDeel"
			description="<li>Developed web applications using NextJS for the frontend and GraphQL with Flask for the backend.</li>
			<li>Managed GitHub Actions for CI/CD pipelines and wrote Terraform configurations to automate infrastructure deployment.</li>
			"
			span={4}
			bgColor="#ff6633"
			time="Apr 2024 - Present"
		/>
		<Chip
			title="Software Developer Intern - Equnix Business Solutions, PT."
			description="<li>Developed ETL tools used to migrate between databases.</li>
			<li>Helped in developing a PostgreSQL extension using C language.</li>
			<li>Analyze and helped to develop POS linux image.</li>
			<li>Contributed to POS management web application backend using Golang</li>
			"
			span={4}
			bgColor="#f7941e"
			time="May 2023 - Aug 2023"
		/>
		<Chip
			title="Distributed System Laboratory Asistant - Institut Teknologi Bandung"
			description="<li>Assisted in IF3130 Computer Networks, IF2230 Operating System, IF2130 Computer Organization and Architecture, and II2130 Computer Architecture and Systems.</li>
			<li>Responsible for giving practicums and assignments to students.</li>
			"
			span={4}
			bgColor="#ff99cc"
			time="July 2022 - Present"
		/>
	</div>
</section>

<style lang="postcss">
</style>
