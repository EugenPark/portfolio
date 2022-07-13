<script lang="ts">
	export let theme = 'light';
	let light = '☀️';
	let dark = '🌙';

	function handleClick(event: any) {
		const html = document.querySelector('html');

		const target = event.target;
		const state = target.checked;
		theme = state ? 'dark' : 'light';
		if (theme === 'dark') {
			html?.classList.add('dark');
		} else {
			html?.classList.remove('dark');
		}
	}
</script>

<!-- Rounded switch -->
<div class="flex gap-2 my-auto">
	<span class="my-auto text-sm font-medium">{light}</span>
	<label for="checked-toggle" class="inline-flex relative items-center cursor-pointer">
		<input
			type="checkbox"
			id="checked-toggle"
			class="sr-only peer"
			on:change={(e) => {
				handleClick(e);
			}}
		/>
		<div
			class="w-11 h-6 bg-blueMunsell dark:bg-lightCoral rounded-full peer peer-focus:ring-4 peer-focus:ring-darkSienna dark:peer-focus:ring-darkSienna  peer-checked:after:translate-x-full peer-checked:after:border-[white] after:content-[''] after:absolute after:top-0.5 after:left-[2px] after:bg-[white] after:border-[white] after:border after:rounded-full after:h-5 after:w-5 after:transition-all"
		/>
	</label>
	<span class="my-auto text-sm font-medium">{dark}</span>
</div>
