<script>
	import Avatar from '$lib/components/Avatar.svelte';
	import Partenaire from '$lib/components/Partenaire.svelte';
	import * as Carousel from '$lib/components/ui/carousel/';

	import BaniereAccueil from '../lib/assets/BanniereAccueil.jpg';

	let AvatarImg =
		'https://avataaars.io/?avatarStyle=Circle&topType=ShortHairShortFlat&accessoriesType=Wayfarers&hairColor=BrownDark&facialHairType=MoustacheMagnum&facialHairColor=Blonde&clotheType=BlazerSweater&eyeType=Default&eyebrowType=RaisedExcited&mouthType=Smile&skinColor=Pale';
</script>

<svelte:head>
	<title>El Cep</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<!-- Baniere-->
<section class="">
	<img src={BaniereAccueil} alt="" class="w-full" />
</section>

<!-- Programtation-->
<section class="bg-slate-200 flex flex-col lg:flex-row items-center lg:items-stretch p-12">
	<div class="w-1/2 flex flex-col items-center mr-4">
		<h1 class="text-5xl font-rock">Vendredi</h1>
		<br />
		<div class="flex m-auto">
			<div class="mr-16">
				<Avatar {AvatarImg} Name="The odd berries"></Avatar>
			</div>
			<div class="ml-16">
				<Avatar {AvatarImg} Name="Boneskaker"></Avatar>
			</div>
		</div>
	</div>
	<div class="w-1/2 flex flex-col items-center ml-4">
		<h1 class="text-5xl font-rock">Samedi</h1>
		<br />
		<div class="flex justify-between">
			<div class="flex flex-col justify-between mr-12">
				<Avatar {AvatarImg} Name="Nobody’s fault" Style=""></Avatar>
				<Avatar {AvatarImg} Name="Ady one women band" Style=""></Avatar>
			</div>
			<div class="flex flex-col justify-center mr-6 ml-6">
				<Avatar {AvatarImg} Name="BB michels" Style=""></Avatar>
			</div>
			<div class="flex flex-col justify-between ml-12">
				<Avatar {AvatarImg} Name="Johnny Montreuil" Style=""></Avatar>
				<Avatar {AvatarImg} Name="DJ ordoeuvre" Style=""></Avatar>
			</div>
		</div>
	</div>
</section>

<!-- Parteneria-->
<section class="flex flex-col items-center w-full p-12">
	<h1 class="text-5xl font-rock mb-8">Partenaires</h1>
	<Carousel.Root opts={{ align: 'start', loop: true }} class="w-5/6">
		<Carousel.Content class="-ml-1">
			<Carousel.Item class="pl-1 md:basis-1/3 lg:basis-1/6">
				<Partenaire PartenaireImg={AvatarImg} Name="Credit Mutuel"></Partenaire>
			</Carousel.Item>
			<Carousel.Item class="pl-1 md:basis-1/3 lg:basis-1/6">
				<Partenaire PartenaireImg={AvatarImg} Name="Credit Mutuel"></Partenaire>
			</Carousel.Item>
			<Carousel.Item class="pl-1 md:basis-1/3 lg:basis-1/6">
				<Partenaire PartenaireImg={AvatarImg} Name="Credit Mutuel"></Partenaire>
			</Carousel.Item>
			<Carousel.Item class="pl-1 md:basis-1/3 lg:basis-1/6">
				<Partenaire PartenaireImg={AvatarImg} Name="Credit Mutuel"></Partenaire>
			</Carousel.Item>
			<Carousel.Item class="pl-1 md:basis-1/3 lg:basis-1/6">
				<Partenaire PartenaireImg={AvatarImg} Name="Credit Mutuel"></Partenaire>
			</Carousel.Item>
			<Carousel.Item class="pl-1 md:basis-1/3 lg:basis-1/6">
				<Partenaire PartenaireImg={AvatarImg} Name="Credit Mutuel"></Partenaire>
			</Carousel.Item>
			<Carousel.Item class="pl-1 md:basis-1/3 lg:basis-1/6">
				<Partenaire PartenaireImg={AvatarImg} Name="Credit Mutuel"></Partenaire>
			</Carousel.Item>
		</Carousel.Content>
		<Carousel.Previous />
		<Carousel.Next />
	</Carousel.Root>
</section>

<style>
</style>
