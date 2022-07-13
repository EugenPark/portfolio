<script lang="ts">
	import Timebox from './Timebox.svelte';
</script>

<div class="flex flex-col gap-2 break-words">
	<h2 class="underline text-2xl text-mint dark:text-[white] font-bold">Education</h2>
	<ol class="relative border-l border-mint dark:border-gray-700">
		<Timebox
			timeIntervall="November 2021 - Today"
			role="Freelancing Software Engineer"
			location="Megatronik"
			description="Creating websites, IT-support and costumer aquisition. Working with technologies such as
            PHP, JavaScript, Python."
			link={true}
		/>
		<Timebox
			timeIntervall="March 2021 - October 2021"
			role="Working Student"
			location="AKKA"
			description="Worked on a Project with Siemens to create a railworker warning system. Used technologies
            such as C++, bash/ shell scripting, linux."
		/>
		<Timebox
			timeIntervall="October 2019 - December 2022"
			role="Student: Information Systems B. Sc."
			location="University of Cologne"
			description="Gaining experiences in the field of computer science aswell as economy. First practical
            experience in Capstone Project working on a real life Project with @Shiftspace to create a
            peer to peer social interactivity app."
		/>
		<Timebox
			timeIntervall="July 2011 - Mai 2019"
			role="Abiture"
			location="Norbert-Gymnasium Knechtsteden"
			description="Final Grade: 1.5"
			lastItem={true}
		/>
	</ol>
</div>
