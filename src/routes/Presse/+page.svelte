<script>
	import * as Tabs from '$lib/components/ui/tabs';
	import BaniereAccueil from '../../lib/assets/Banniere.jpg';
	import Groupe from '../../lib/components/Groupe.svelte';
	import ImgGroupe from '../../lib/assets/ELCEP_logo_festival.png';
	import Icon from '@iconify/svelte';

	import Presses from '$lib/Presse.json';

</script>

<!-- Baniere-->
<section class="">
	<img src={BaniereAccueil} alt="" class="w-full" />
</section>

<section class="flex justify-center items-center flex-col mt-8">
	
			<h1 class="font-rock text-3xl mb-4">2024</h1>
			{#each Presses.filter((e) => e.Year == "2024") as Presse}
			<div class="flex flex-col items-center justify-center bg-gray-100 rounded-md p-4 gap-8 w-4/6">
				<a class="font-rock text-2xl hover:underline" href={Presse.Url}>{Presse['Title ']}</a> 
			</div>
			<br />
			{/each}
	
			<h1 class="font-rock text-3xl mb-4">2023</h1>
			{#each Presses.filter((e) => e.Year == "2023") as Presse}
			<div class="flex flex-col items-center justify-center bg-gray-100 rounded-md p-4 gap-8 w-4/6">
				<a class="font-rock text-2xl hover:underline" href={Presse.Url}>{Presse['Title ']}</a> 
			</div>
			<br />
			{/each}

			<h1 class="font-rock text-3xl mb-4">2022</h1>
			{#each Presses.filter((e) => e.Year == "2022") as Presse}
			<div class="flex flex-col items-center justify-center bg-gray-100 rounded-md p-4 gap-8 w-4/6">
				<a class="font-rock text-2xl hover:underline" href={Presse.Url}>{Presse['Title ']}</a> 
			</div>
			<br />
			{/each}

			<h1 class="font-rock text-3xl mb-4">2019</h1>
			{#each Presses.filter((e) => e.Year == "2019") as Presse}
			<div class="flex flex-col items-center justify-center bg-gray-100 rounded-md p-4 gap-8 w-4/6">
				<a class="font-rock text-2xl hover:underline" href={Presse.Url}>{Presse['Title ']}</a> 
			</div>
			<br />
			{/each}

			<h1 class="font-rock text-3xl mb-4">2018</h1>
			{#each Presses.filter((e) => e.Year == "2018") as Presse}
			<div class="flex flex-col items-center justify-center bg-gray-100 rounded-md p-4 gap-8 w-4/6">
				<a class="font-rock text-2xl hover:underline" href={Presse.Url}>{Presse['Title ']}</a> 
			</div>
			<br />
			{/each}
</section>
