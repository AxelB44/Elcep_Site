<script>
	import * as Tabs from '$lib/components/ui/tabs';
	import BaniereAccueil from '../../lib/assets/BanniereAccueil.jpg';
	import Groupe from '../../lib/components/Groupe.svelte';
	import ImgGroupe from '../../lib/assets/ELCEP_logo_festival.png';
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
			<Groupe Img={ImgGroupe}>
				<h1 slot="name" class="font-rock text-2xl m-2">The odd berries</h1>
				<h2 slot="style" class="text-xl m-2">Test</h2>
				<p slot="description" class="text-justify m-2">
					Le Lorem Ipsum est simplement du faux texte employé dans la composition et la mise en page
					avant impression. Le Lorem Ipsum est le faux texte standard de l'imprimerie depuis les
					années 1500, quand un imprimeur anonyme assembla ensemble des morceaux de texte pour
					réaliser un livre spécimen de polices de texte. Il n'a pas fait que survivre cinq siècles,
					mais s'est aussi adapté à la bureautique informatique, sans que son contenu n'en soit
					modifié. Il a été popularisé dans les années 1960 grâce à la vente de feuilles Letraset
					contenant des passages du Lorem Ipsum, et, plus récemment, par son inclusion dans des
					applications de mise en page de texte, comme Aldus PageMaker.
				</p>
			</Groupe>
			<br />
			<Groupe Img={ImgGroupe}>
				<h1 slot="name" class="font-rock text-2xl m-2">Boneskaker</h1>
				<h2 slot="style" class="text-xl m-2">Test</h2>
				<p slot="description" class="text-justify m-2">
					Le Lorem Ipsum est simplement du faux texte employé dans la composition et la mise en page
					avant impression. Le Lorem Ipsum est le faux texte standard de l'imprimerie depuis les
					années 1500, quand un imprimeur anonyme assembla ensemble des morceaux de texte pour
					réaliser un livre spécimen de polices de texte. Il n'a pas fait que survivre cinq siècles,
					mais s'est aussi adapté à la bureautique informatique, sans que son contenu n'en soit
					modifié. Il a été popularisé dans les années 1960 grâce à la vente de feuilles Letraset
					contenant des passages du Lorem Ipsum, et, plus récemment, par son inclusion dans des
					applications de mise en page de texte, comme Aldus PageMaker.
				</p>
			</Groupe>
			<br />
		</Tabs.Content>

		<Tabs.Content value="Samedi">
			<Groupe Img={ImgGroupe}>
				<h1 slot="name" class="font-rock text-2xl m-2">Nobody’s fault</h1>
				<h2 slot="style" class="text-xl m-2">Test</h2>
				<p slot="description" class="text-justify m-2">
					Le Lorem Ipsum est simplement du faux texte employé dans la composition et la mise en page
					avant impression. Le Lorem Ipsum est le faux texte standard de l'imprimerie depuis les
					années 1500, quand un imprimeur anonyme assembla ensemble des morceaux de texte pour
					réaliser un livre spécimen de polices de texte. Il n'a pas fait que survivre cinq siècles,
					mais s'est aussi adapté à la bureautique informatique, sans que son contenu n'en soit
					modifié. Il a été popularisé dans les années 1960 grâce à la vente de feuilles Letraset
					contenant des passages du Lorem Ipsum, et, plus récemment, par son inclusion dans des
					applications de mise en page de texte, comme Aldus PageMaker.
				</p>
			</Groupe>
			<br />
			<Groupe Img={ImgGroupe}>
				<h1 slot="name" class="font-rock text-2xl m-2">Ady one women band</h1>
				<h2 slot="style" class="text-xl m-2">Test</h2>
				<p slot="description" class="text-justify m-2">
					Le Lorem Ipsum est simplement du faux texte employé dans la composition et la mise en page
					avant impression. Le Lorem Ipsum est le faux texte standard de l'imprimerie depuis les
					années 1500, quand un imprimeur anonyme assembla ensemble des morceaux de texte pour
					réaliser un livre spécimen de polices de texte. Il n'a pas fait que survivre cinq siècles,
					mais s'est aussi adapté à la bureautique informatique, sans que son contenu n'en soit
					modifié. Il a été popularisé dans les années 1960 grâce à la vente de feuilles Letraset
					contenant des passages du Lorem Ipsum, et, plus récemment, par son inclusion dans des
					applications de mise en page de texte, comme Aldus PageMaker.
				</p>
			</Groupe>
			<br />
			<Groupe Img={ImgGroupe}>
				<h1 slot="name" class="font-rock text-2xl m-2">BB michels</h1>
				<h2 slot="style" class="text-xl m-2">Test</h2>
				<p slot="description" class="text-justify m-2">
					Le Lorem Ipsum est simplement du faux texte employé dans la composition et la mise en page
					avant impression. Le Lorem Ipsum est le faux texte standard de l'imprimerie depuis les
					années 1500, quand un imprimeur anonyme assembla ensemble des morceaux de texte pour
					réaliser un livre spécimen de polices de texte. Il n'a pas fait que survivre cinq siècles,
					mais s'est aussi adapté à la bureautique informatique, sans que son contenu n'en soit
					modifié. Il a été popularisé dans les années 1960 grâce à la vente de feuilles Letraset
					contenant des passages du Lorem Ipsum, et, plus récemment, par son inclusion dans des
					applications de mise en page de texte, comme Aldus PageMaker.
				</p>
			</Groupe>
			<br />
			<Groupe Img={ImgGroupe}>
				<h1 slot="name" class="font-rock text-2xl m-2">Johnny Montreuil</h1>
				<h2 slot="style" class="text-xl m-2">Test</h2>
				<p slot="description" class="text-justify m-2">
					Le Lorem Ipsum est simplement du faux texte employé dans la composition et la mise en page
					avant impression. Le Lorem Ipsum est le faux texte standard de l'imprimerie depuis les
					années 1500, quand un imprimeur anonyme assembla ensemble des morceaux de texte pour
					réaliser un livre spécimen de polices de texte. Il n'a pas fait que survivre cinq siècles,
					mais s'est aussi adapté à la bureautique informatique, sans que son contenu n'en soit
					modifié. Il a été popularisé dans les années 1960 grâce à la vente de feuilles Letraset
					contenant des passages du Lorem Ipsum, et, plus récemment, par son inclusion dans des
					applications de mise en page de texte, comme Aldus PageMaker.
				</p>
			</Groupe>
			<br />
			<Groupe Img={ImgGroupe}>
				<h1 slot="name" class="font-rock text-2xl m-2">DJ ordoeuvre</h1>
				<h2 slot="style" class="text-xl m-2">Test</h2>
				<p slot="description" class="text-justify m-2">
					Le Lorem Ipsum est simplement du faux texte employé dans la composition et la mise en page
					avant impression. Le Lorem Ipsum est le faux texte standard de l'imprimerie depuis les
					années 1500, quand un imprimeur anonyme assembla ensemble des morceaux de texte pour
					réaliser un livre spécimen de polices de texte. Il n'a pas fait que survivre cinq siècles,
					mais s'est aussi adapté à la bureautique informatique, sans que son contenu n'en soit
					modifié. Il a été popularisé dans les années 1960 grâce à la vente de feuilles Letraset
					contenant des passages du Lorem Ipsum, et, plus récemment, par son inclusion dans des
					applications de mise en page de texte, comme Aldus PageMaker.
				</p>
			</Groupe>
			<br />
		</Tabs.Content>
	</Tabs.Root>
</section>
