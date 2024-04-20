<script>
	import Banniere from '../../lib/assets/Banniere.jpg';

	import * as Tabs from '$lib/components/ui/tabs';
	import Groupe from '../../lib/components/Groupe.svelte';
	import ImgGroupe from '../../lib/assets/ELCEP_logo_festival.png';
</script>

<section class="">
	<img src={Banniere} alt="" class="w-full" />
</section>

<section class="flex justify-center items-center">
	<Tabs.Root value="Localisation" class="w-5/6 flex flex-col m-4">
		<Tabs.List class="mb-4">
			<Tabs.Trigger value="Localisation" class="font-rock text-xl md:text-3xl">Localisation</Tabs.Trigger>
			<Tabs.Trigger value="Restauration" class="font-rock text-xl md:text-3xl">Restauration</Tabs.Trigger>
			<Tabs.Trigger value="Campings" class="font-rock text-xl md:text-3xl">Camping</Tabs.Trigger>
		</Tabs.List>
		<Tabs.Content value="Localisation">
			<div class="flex md:flex-row flex-col items-center justify-center bg-gray-100 rounded-md p-4 gap-8">
				<iframe
					src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d5423.442135823497!2d-1.7121883470627746!3d47.510665762199295!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x480f612db85ae8e9%3A0x3d3aa7bafca1b46a!2sLe%20Cep%2C%2044170%20La%20Grigonnais!5e1!3m2!1sfr!2sfr!4v1713610958714!5m2!1sfr!2sfr"
					class="w-full h-[600px] md:w-1/2"
					style="border:0;"
					title="Localisation el cep via map"
					allowfullscreen={true}
					loading="lazy"
					referrerpolicy="no-referrer-when-downgrade"
				></iframe>
				<div class="md:w-1/2">
				<p class="text-justify m-2">Le festival est situé dans le village Le Cep à La Grigonnais (44170) en Loire Atlantique, à environ 30 km au nord de Nantes.</p>
				</div>
			</div>
			<br />
			<div class="flex flex-col items-center justify-center bg-gray-100 rounded-md p-4 gap-8">
				<h1 class="font-rock text-2xl m-2">Parking</h1>
				<p class="text-justify m-2">Dès les entrées de La Grigonnais, l'entrée du festival est indiquée par des panneaux de signalétique. Un grand parking est mis à disposition des festivaliers qui comptent repartir dans la soirée.</p>
			</div>
		</Tabs.Content>

		<Tabs.Content value="Restauration">
			<div class="flex flex-col items-center justify-center bg-gray-100 rounded-md p-4 gap-8">
				<h1 class="font-rock text-2xl m-2">Restauration sur place</h1>
				<p class="text-justify m-2">Sur le site du festival, nos bénévoles de la restauration se feront un plaisir de vous servir façon snacking !</p>
			</div>
			<br />
		</Tabs.Content>

		<Tabs.Content value="Campings">
			<div class="flex flex-col items-center justify-center bg-gray-100 rounded-md p-4 gap-8">
				<h1 class="font-rock text-2xl m-2">Camping a dispotition</h1>
				<p class="text-justify m-2">Un camping est à disposition des festivaliers qui souhaitent profiter de leur soirée en toute sécurité. L'accès au terrain est indiqué par des panneaux de signalétique sur site.</p>
			</div>
			<br />
		</Tabs.Content>
	</Tabs.Root>
</section>
