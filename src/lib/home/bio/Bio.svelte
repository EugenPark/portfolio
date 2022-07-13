<script lang="ts">
	import Timeline from './timeline/Timeline.svelte';
</script>

<div class="m-auto flex flex-col gap-9 dark:text-[white]">
	<div
		class="block p-4  bg-jetStream rounded-3xl border border-jetStream shadow-md  dark:bg-blueMunsell dark:border-blueMunsell dark:hover:bg-gray-700"
	>
		<h5 class="mb-2 text-xl font-bold tracking-tight text-gray-900 dark:text-white">
			Hello, World!
		</h5>
		<p class="font-normal text-gray-700 dark:text-gray-400">
			Thank you for visiting my portfolio page. I hope you enjoy the stay!
		</p>
	</div>
	<div class="flex gap-5 ">
		<div class="my-auto">
			<h3 class="text-xl font-bold">Eugene Park</h3>
			<p>Studying Information Systems B. Sc. at University of Cologne</p>
		</div>
		<img class="rounded-full w-32 h-28" src="/docs/images/profile.jpeg" alt="Profile picture" />
	</div>
	<div class="flex flex-col gap-2 break-words">
		<h2 class="underline text-2xl text-mint dark:text-[white] font-bold">About Me</h2>
		<p class="">
			Information Systems Bsc student at the University of Cologne. Experience in Computer
			Engineering as a working student at AKKA Technologies Cologne. Programming skills in Java and
			Python. Speaking 4 languages (German, English, Lithuanian, Korean). Currently playing for the
			U21 Lithuanian National Football Team.
		</p>
	</div>
	<Timeline />
	<div class="flex flex-col gap-2">
		<h2 class="underline text-2xl text-mint dark:text-[white] font-bold">Projects</h2>
		<p class="break-words">
			Lorem ipsum dolor sit amet, consectetur adipisicing elit. Autem enim unde voluptates? Delectus
			ex distinctio tempore placeat ipsum, rerum, perspiciatis, saepe autem quisquam velit
			laudantium porro culpa debitis sed repudiandae.
		</p>
	</div>
</div>
