<script lang="ts">
	export let logos: string[] = [];
	export let logo: string = '';
	export let title: string;
	export let description: string;
	export let span: number = 1;
	export let bgColor: string = '#9966bb';
	if (logos.length == 0 && logo != '') {
		logos = [logo];
	}
	export let link: string = '';
	export let time: string = '';
</script>

<div
	class="language-container"
	style="background-color: {bgColor}88; grid-column: span {span} / span {span}"
>
	<div class="flex items-center">
		{#each logos as logo}
			<img src={logo} alt="Python" class="w-4 h-4 mr-2" />
		{/each}
		<div class="w-full flex justify-between items-center">
			{#if link}
				<a href={link} class="external"><h3>{title}</h3></a>
			{:else}
				<h3>{title}</h3>
			{/if}
			{#if time}
				<p class="text-xs text-gray-600">{time}</p>
			{/if}
		</div>
	</div>
	<p>{description}</p>
</div>

<style lang="postcss">
	.language-container {
		padding: 16px;
		border-radius: 12px;
	}
	h3 {
		font-weight: 700;
	}
	.external {
		background-image: url('/icons/external-link.png');
		background-position: center right;
		background-repeat: no-repeat;
		background-size: 0.857em;
		padding-right: 1rem;
		color: #3366cc;
	}
</style>
