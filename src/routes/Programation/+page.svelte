<script>
	import * as Tabs from '$lib/components/ui/tabs';
	import BaniereAccueil from '../../lib/assets/BanniereAccueil.jpg';
	import Groupe from '../../lib/components/Groupe.svelte';
	import ImgGroupe from '../../lib/assets/ELCEP_logo_festival.png';
	import Icon from '@iconify/svelte';

	import Artistes from '$lib/Artiste.json';
</script>

<!-- Baniere-->
<section class="">
	<img src={BaniereAccueil} alt="" class="w-full" />
</section>

<section class="flex justify-center items-center">
	<Tabs.Root value="Vendredi" class="w-5/6 flex flex-col m-4">
		<Tabs.List class="mb-4">
			<Tabs.Trigger value="Vendredi" class="font-rock text-3xl">Vendredi</Tabs.Trigger>
			<Tabs.Trigger value="Samedi" class="font-rock text-3xl">Samedi</Tabs.Trigger>
		</Tabs.List>
		<Tabs.Content value="Vendredi">
			{#each Artistes.filter((e) => e.Date == 'Vendredi') as Artiste}
				<Groupe Img={Artiste.Image} Reseaux={Artiste.Reseaux}>
					<h1 slot="name" class="font-rock text-2xl m-2">{Artiste.Name}</h1>
					<p slot="description" class="text-justify m-2">{Artiste.Description}</p>
				</Groupe>
				<br />
			{/each}
		</Tabs.Content>

		<Tabs.Content value="Samedi">
			{#each Artistes.filter((e) => e.Date == 'Samedi') as Artiste}
				<Groupe Img={Artiste.Image} Reseaux={Artiste.Reseaux}>
					<h1 slot="name" class="font-rock text-2xl m-2">{Artiste.Name}</h1>
					<p slot="description" class="text-justify m-2">{Artiste.Description}</p>
				</Groupe>
				<br />
			{/each}
		</Tabs.Content>
	</Tabs.Root>
</section>
