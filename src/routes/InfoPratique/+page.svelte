<script>
	import Baniere from '../../lib/assets/BanniereAccueil.jpg';
	import * as Tabs from '$lib/components/ui/tabs';
	import Groupe from '../../lib/components/Groupe.svelte';
	import ImgGroupe from '../../lib/assets/ELCEP_logo_festival.png';
</script>

<section class="">
	<img src={Baniere} alt="" class="w-full" />
</section>

<section class="flex justify-center items-center">
	<Tabs.Root value="Localisation" class="w-5/6 flex flex-col m-4">
		<Tabs.List class="mb-4">
			<Tabs.Trigger value="Localisation" class="font-rock text-3xl">Localisation</Tabs.Trigger>
			<Tabs.Trigger value="Restauration" class="font-rock text-3xl">Restauration</Tabs.Trigger>
			<Tabs.Trigger value="Campings" class="font-rock text-3xl">Camping</Tabs.Trigger>
		</Tabs.List>
		<Tabs.Content value="Localisation">
			<Groupe Img={ImgGroupe}>
				<h1 slot="name" class="font-rock text-2xl m-2">Le Cep - La grigonnais 44170</h1>
				<p slot="description" class="text-justify m-2"></p>
			</Groupe>
			<br />
		</Tabs.Content>

		<Tabs.Content value="Restauration">
			<Groupe Img={ImgGroupe}>
				<h1 slot="name" class="font-rock text-2xl m-2">Restauration sur place</h1>
				<p slot="description" class="text-justify m-2"></p>
			</Groupe>
			<br />
		</Tabs.Content>

		<Tabs.Content value="Campings">
			<Groupe Img={ImgGroupe}>
				<h1 slot="name" class="font-rock text-2xl m-2">Camping a dispotition</h1>
				<p slot="description" class="text-justify m-2"></p>
			</Groupe>
			<br />
		</Tabs.Content>
	</Tabs.Root>
</section>
