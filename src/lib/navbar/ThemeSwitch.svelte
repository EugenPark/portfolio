<script lang="ts">
	export let value = 'off';
	let light = '☀️';
	let dark = '🌙';
	let checked = true;

	function handleClick(event: any) {
		const target = event.target;
		const state = target.getAttribute('aria-checked');
		checked = state === 'true' ? false : true;
		value = checked === true ? 'on' : 'off';
	}
</script>

<!-- Rounded switch -->
<div class="flex gap-2 my-auto">
	<span class="my-auto text-sm font-medium">{dark}</span>
	<label for="checked-toggle" class="inline-flex relative items-center cursor-pointer">
		<input type="checkbox" value="" id="checked-toggle" class="sr-only peer" checked />
		<div
			class="w-11 h-6 bg-[#ccc] rounded-full peer peer-focus:ring-4 peer-focus:ring-skyBlueCrayola dark:peer-focus:ring-skyBlueCrayola dark:bg-[black] peer-checked:after:translate-x-full peer-checked:after:border-[white] after:content-[''] after:absolute after:top-0.5 after:left-[2px] after:bg-[white] after:border-[white] after:border after:rounded-full after:h-5 after:w-5 after:transition-all dark:border-[#ccc] peer-checked:bg-skyBlueCrayola"
		/>
	</label>
	<span class="my-auto text-sm font-medium">{light}</span>
</div>
