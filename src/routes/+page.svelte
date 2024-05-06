<script>
	import Avatar from '$lib/components/Avatar.svelte';
	import Partenaire from '$lib/components/Partenaire.svelte';
	import * as Carousel from '$lib/components/ui/carousel/';
	import Autoplay from 'embla-carousel-autoplay';

	import BanniereAccueil from '../lib/assets/BanniereAccueil.png';
	import lPartenaires from '$lib/Partenaire.json';

	const plugin = Autoplay({ delay: 3000, stopOnInteraction: true });
</script>

<svelte:head>
	<title>El Cep : Festival Rock à La Grigonnais (44) - 6 & 7 septembre 2024</title>
	<meta
		name="description"
		content="Le festival El Cep est de retour pour sa 5ème édition et vous promet un week-end inoubliable placé sous le signe du rock ! Du vendredi 6 septembre au samedi 7 septembre 2024, le village de La Grigonnais va vibrer au rythme des guitares et des voix puissantes."
	/>
	<meta
		name="keywords"
		content="festival, rock, musique, La Grigonnais, El Cep,ElCep, concert, programmation, billetterie, événement, France"
	/>
	<meta name="viewport" content="width=device-width, initial-scale=1.0" />
	<meta charset="UTF-8" />
	<meta name="robots" content="index, follow" />
</svelte:head>

<!-- Baniere-->
<section class="">
	<img src={BanniereAccueil} alt="" class="w-full" />
</section>

<!-- Programtation-->
<section class="bg-gray-100 flex flex-col lg:flex-row items-center lg:items-stretch p-8">
	<div class="w-1/2 flex flex-col items-center mb-8">
		<h1 class="text-5xl font-rock text-nowrap">Vendredi 6 Sept</h1>
		<br />
		<div class="flex mt-auto mb-auto">
			<div class="mr-6">
				<Avatar AvatarImg="../Artiste/OddBerris/ODDBERRIESAvatar.jpg" Name="Odd berries"
				></Avatar>
			</div>
			<div class="ml-6">
				<Avatar AvatarImg="../Artiste/BoneShaker/avatar_boneshaker.jpg" Name="BoneShaker"></Avatar>
			</div>
		</div>
	</div>
	<div class="w-1/2 flex flex-col items-center">
		<h1 class="text-5xl font-rock text-nowrap">Samedi 7 Sept</h1>
		<br />
		<div class="flex flex-row justify-between items-center lg:gap-16">
			<div class="flex flex-col justify-between">
				<Avatar AvatarImg="../Artiste/NobodysFault/avatar_nobody.jpg" Name="Nobody’s fault"
				></Avatar>
				<Avatar AvatarImg="../Artiste/AdyOneWomenband/adyowbAvatar.jpg" Name="Ady One Woman Band"
				></Avatar>
			</div>
			<div class="flex flex-col justify-center">
				<Avatar AvatarImg="../Artiste/BBMichels/BBMichelsAvatars.jpg" Name="Broken Back Michels"></Avatar>
			</div>
			<div class="flex flex-col justify-between">
				<Avatar AvatarImg="../Artiste/JohnnyMontreuil/avatar_jm2.png" Name="Johnny Montreuil"
				></Avatar>
				<Avatar AvatarImg="../Artiste/DJOrdoeuvre/avatar_djordoeuvre2.jpg" Name="DJ ordoeuvre"
				></Avatar>
			</div>
		</div>
	</div>
</section>

<!-- Parteneria-->
<section class="flex flex-col items-center w-full p-12">
	<h1 class="text-5xl font-rock mb-8">Partenaires</h1>
	<Carousel.Root opts={{ align: 'start', loop: true }} plugins={[plugin]} class="w-5/6">
		<Carousel.Content class="-ml-1">
			{#each lPartenaires as oPartenaire}
				<Carousel.Item class="pl-1 basis-1/2 md:basis-1/3 lg:basis-1/6">
					<Partenaire PartenaireImg={oPartenaire.Image} Name={oPartenaire.Name}></Partenaire>
				</Carousel.Item>
			{/each}
		</Carousel.Content>
		<Carousel.Previous />
		<Carousel.Next />
	</Carousel.Root>
</section>
