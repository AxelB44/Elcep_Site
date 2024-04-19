<script>
	import Avatar from '$lib/components/Avatar.svelte';
	import Partenaire from '$lib/components/Partenaire.svelte';
	import * as Carousel from '$lib/components/ui/carousel/';
	import Autoplay from 'embla-carousel-autoplay';
	
	import BaniereAccueil from '../lib/assets/BanniereAccueil.jpg';
	import lPartenaires from '$lib/Partenaire.json'

	let AvatarImg =
		'https://avataaars.io/?avatarStyle=Circle&topType=ShortHairShortFlat&accessoriesType=Wayfarers&hairColor=BrownDark&facialHairType=MoustacheMagnum&facialHairColor=Blonde&clotheType=BlazerSweater&eyeType=Default&eyebrowType=RaisedExcited&mouthType=Smile&skinColor=Pale';

	
	const plugin = Autoplay({ delay: 3000, stopOnInteraction: true });
</script>

<svelte:head>
	<title>El Cep</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<!-- Baniere-->
<section class="">
	<img src={BaniereAccueil} alt="" class="w-full object-right-top object-cover lg:object-fill" />
</section>

<!-- Programtation-->
<section class="bg-gray-100 flex flex-col lg:flex-row items-center lg:items-stretch p-8">
	<div class="w-1/2 flex flex-col items-center mb-8">
		<h1 class="text-5xl font-rock text-nowrap">Vendredi 06/09</h1>
		<br />
		<div class="flex mt-auto mb-auto">
			<div class="mr-6">
				<Avatar AvatarImg='../Artiste/OddBerris/ODD BERRIES Avatar.jpg' Name="The odd berries"></Avatar>
			</div>
			<div class="ml-6">
				<Avatar AvatarImg='../Artiste/BoneShaker/avatar_boneshaker.jpg' Name="Boneskaker"></Avatar>
			</div>
		</div>
	</div>
	<div class="w-1/2 flex flex-col items-center">
		<h1 class="text-5xl font-rock">Samedi 07/09</h1>
		<br />
		<div class="flex flex-row justify-between items-center">
			<div class="flex flex-col justify-between mr-6">
				<Avatar AvatarImg='../Artiste/NobodysFault/avatar_nobody.jpg' Name="Nobody’s fault"></Avatar>
				<Avatar AvatarImg='../Artiste/AdyOneWomenband/adyowbAvatar.jpg' Name="Ady one women band"></Avatar>
			</div>
			<div class="flex flex-col justify-center m-6">
				<Avatar AvatarImg='../Artiste/BBMichels/' Name="BB michels"></Avatar>
			</div>
			<div class="flex flex-col justify-between ml-6">
				<Avatar AvatarImg='../Artiste/JohnnyMontreuil/avatar_jm2.png' Name="Johnny Montreuil"></Avatar>
				<Avatar AvatarImg='../Artiste/DJOrdoeuvre/avatar_djordoeuvre2.jpg' Name="DJ ordoeuvre"></Avatar>
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
				<Carousel.Item class="pl-1 md:basis-1/3 lg:basis-1/6">
				<Partenaire PartenaireImg={oPartenaire.Image}  Name={oPartenaire.Name}></Partenaire>
			</Carousel.Item>
			{/each}
		</Carousel.Content>
		<Carousel.Previous />
		<Carousel.Next />
	</Carousel.Root>
</section>

