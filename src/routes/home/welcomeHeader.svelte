<script lang="ts">
	let index: number = 0;
	let hello: string[] = ['hello', 'labas', 'hallo'];
	setInterval(() => {
		if (index + 1 < hello.length) {
			index++;
		} else {
			index = 0;
		}
	}, 2000);
</script>

<div class="content">
	<h1>{hello[index]}, world!</h1>
</div>

<style>
	h1 {
		margin: auto;
	}
</style>
