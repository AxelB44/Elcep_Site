<script>
	import Avatar from '$lib/components/Avatar.svelte';
	import Partenaire from '$lib/components/Partenaire.svelte';
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
<section class="bg-slate-200 flex p-2">
	<div class="w-1/2 flex flex-col items-center">
		<h1 class="text-3xl font-rock">Vendredi</h1>
		<br />
		<div class="flex m-auto">
			<Avatar {AvatarImg} Name="The odd berries" Style=""></Avatar>
			<Avatar {AvatarImg} Name="Boneskaker" Style=""></Avatar>
		</div>
	</div>
	<div class="w-1/2 flex flex-col items-center">
		<h1 class="text-3xl font-rock">Samedi</h1>
		<br />
		<div class="grid grid-cols-3">
			<Avatar {AvatarImg} Name="Nobody’s fault" Style=""></Avatar>
			<Avatar {AvatarImg} Name="Ady one women band" Style=""></Avatar>
			<Avatar {AvatarImg} Name="BB michels" Style=""></Avatar>
			<Avatar {AvatarImg} Name="Johnny Montreuil" Style=""></Avatar>
			<Avatar {AvatarImg} Name="DJ ordoeuvre" Style=""></Avatar>
		</div>
	</div>
</section>

<!-- Parteneria-->
<section class="flex flex-col items-center p-2">
	<h1 class="text-4xl font-rock">Partenaires</h1>
	<div class="flex">
		<Partenaire PartenaireImg={AvatarImg} Name="Credit Mutuel"></Partenaire>
		<Partenaire PartenaireImg={AvatarImg} Name="Credit Mutuel"></Partenaire>
		<Partenaire PartenaireImg={AvatarImg} Name="Credit Mutuel"></Partenaire>
	</div>
</section>

<style>
</style>
