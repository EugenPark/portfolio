<script lang="ts">
	export let timeIntervall: string;
	export let role: string;
	export let location: string;
	export let description: string;
	export let link: boolean = false;
	export let lastItem: boolean = false;
</script>

<li class="{lastItem ? '' : 'mb-10'} ml-4">
	<div class="absolute w-3 h-3 bg-mint rounded-full mt-1.5 -left-1.5 border border-mint " />
	<time class="mb-1 text-sm font-normal leading-none ">{timeIntervall}</time>
	<h3 class="text-lg font-semibold ">{role} @ {location}</h3>
	<p class="mb-4 text-base font-normal ">
		{description}
	</p>
	{#if link}
		<a
			href="#"
			class="inline-flex items-center py-2 px-4 text-sm font-medium  bg-mint text-[white] rounded-lg border border-mint focus:z-10 focus:ring-4 focus:outline-none focus:ring-mint"
			>Learn more <svg
				class="ml-2 w-3 h-3"
				fill="currentColor"
				viewBox="0 0 20 20"
				xmlns="http://www.w3.org/2000/svg"
				><path
					fill-rule="evenodd"
					d="M12.293 5.293a1 1 0 011.414 0l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-2.293-2.293a1 1 0 010-1.414z"
					clip-rule="evenodd"
				/></svg
			></a
		>
	{/if}
</li>
