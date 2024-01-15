<script lang="ts">
	import nodejsLogo from '$lib/images/nodedotjs.svg';
	import reactjsLogo from '$lib/images/react.svg';
	import nextjsLogo from '$lib/images/nextdotjs.svg';
	import flutterLogo from '$lib/images/flutter.svg';
	import svelteLogo from '$lib/images/svelte.svg';
	import laravelLogo from '$lib/images/laravel.svg';
	import flaskLogo from '$lib/images/flask.svg';
	import unityLogo from '$lib/images/unity.svg';
	import godotLogo from '$lib/images/godotengine.svg';
	import ubuntuLogo from '$lib/images/ubuntu.svg';
	import debianLogo from '$lib/images/debian.svg';
	import archLogo from '$lib/images/archlinux.svg';
	import dockerLogo from '$lib/images/docker.svg';
	import kubernetesLogo from '$lib/images/kubernetes.svg';
	import postgresLogo from '$lib/images/postgresql.svg';
	import mysqlLogo from '$lib/images/mysql.svg';
	import mongodbLogo from '$lib/images/mongodb.svg';
	import rabbitmqLogo from '$lib/images/rabbitmq.svg';
	import figmaLogo from '$lib/images/figma.svg';

	import Chip from '$lib/components/Chip.svelte';
</script>

<section id="tools">
	<h1 class="font-bold text-lg mb-4">Some Frameworks, Tools, etc. I Have Used</h1>
	<div class="grid grid-cols-2 md:grid-cols-4 gap-2">
		<Chip
			logos={[nodejsLogo, reactjsLogo, nextjsLogo, flutterLogo, svelteLogo]}
			title="Frontend Frameworks"
			description="Node.js, React.js, Next.js, Flutter, Svelte for developing frontend web apps"
			span={2}
			bgColor="#f7df1e"
		/>
		<Chip
			logos={[nodejsLogo, flaskLogo, laravelLogo]}
			title="Backend Frameworks"
			description="Node.js, Express.js, Flask, Laravel for developing backend web apps"
			span={2}
			bgColor="#3776ab"
		/>
		<Chip
			logos={[unityLogo, godotLogo]}
			title="Game Engine"
			description="Unity, Godot for developing games"
			span={2}
			bgColor="#00b4ab"
		/>
		<Chip
			logos={[ubuntuLogo, debianLogo, archLogo]}
			title="Linux Distributions"
			description="Ubuntu, Debian, Arch Linux for linux distributions"
			span={2}
			bgColor="#0095d5"
		/>
		<Chip
			logos={[dockerLogo, kubernetesLogo]}
			title="Containerization"
			description="Docker, Kubernetes for containerization"
			span={2}
			bgColor="#4eaa25"
		/>
		<Chip
			logos={[postgresLogo, mysqlLogo, mongodbLogo]}
			title="Databases"
			description="PostgreSQL, MySQL, MongoDB for databases"
			span={2}
			bgColor="#31648c"
		/>
		<Chip
			logos={[rabbitmqLogo]}
			title="Message Broker"
			description="RabbitMQ for message broker"
			span={2}
			bgColor="#ff6600"
		/>
		<Chip
			logos={[figmaLogo]}
			title="Design Tools"
			description="Figma for design tools"
			span={2}
			bgColor="#f24e1e"
		/>
	</div>
</section>

<style lang="postcss">
</style>
