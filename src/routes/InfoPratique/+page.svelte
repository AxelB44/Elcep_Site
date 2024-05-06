<script>
	import Banniere from '../../lib/assets/Banniere.jpg';

	import * as Tabs from '$lib/components/ui/tabs';
	import ImgRestauration from '$lib/assets/RESTAURATION.png';
	import ImgSurPlace from '$lib/assets/entrefest.jpg';
	import ImgCamping from '$lib/assets/CAMPING.png';
	import ImgEcoFest from '$lib/assets/Eco-fest.jpg';


</script>

<section class="">
	<img src={Banniere} alt="" class="w-full" />
</section>

<section class="flex justify-center items-center">
	<Tabs.Root value="Localisation" class="w-11/12 md:w-5/6 flex flex-col m-4">
		<Tabs.List class="mb-4 h-auto block md:inline-flex" aria-orientation='horizontal'>
			<Tabs.Trigger value="Localisation" class="font-rock text-xl md:text-3xl">Localisation</Tabs.Trigger>
			<Tabs.Trigger value="Sur place" class="font-rock text-xl md:text-3xl">Sur place</Tabs.Trigger>
			<Tabs.Trigger value="Restauration" class="font-rock text-xl md:text-3xl">Restauration</Tabs.Trigger>
			<Tabs.Trigger value="Zone de nuit" class="font-rock text-xl md:text-3xl">Zone de nuit</Tabs.Trigger>
			<Tabs.Trigger value="Eco-Festival" class="font-rock text-xl md:text-3xl">Eco-Festival</Tabs.Trigger>
			<Tabs.Trigger value="FAQ" class="font-rock text-xl md:text-3xl">FAQ</Tabs.Trigger>

		</Tabs.List>

		<Tabs.Content value="Localisation">
			<div
				class="flex md:flex-row flex-col items-center justify-center bg-gray-100 rounded-md p-4 gap-8"
			>
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
					<p class="text-justify m-2">
						Le festival est situé dans le village Le Cep à La Grigonnais (44170) en Loire
						Atlantique, à environ 30 km au nord de Nantes.
					</p>
				</div>
			</div>
			<br />			
			<div class="flex flex-col items-center justify-center bg-gray-100 rounded-md p-4 gap-8">
				<h1 class="font-rock text-2xl m-2">Parking</h1>
				<p class="text-justify m-2">
					Au abords de La Grigonnais, des panneaux de signalisation vous guideront vers le parkings et l'entrée du festival. 
					<br/>
					Un grand parking est situé à proximité du site et est idéal pour ceux qui souhaitent repartir dans la soirée.
				</p>
			</div>
			<br />
			<div class="flex flex-col items-center justify-center bg-gray-100 rounded-md p-4 gap-8">
				<h1 class="font-rock text-2xl m-2">Transport en commun</h1>
				<p class="text-justify m-2">Les lignes Aléop 309 et 310 vous emmènent directement de Nantes à proximité du festival en à peine une heure, pour profiter pleinement de l'ambiance et des festivités.</p>
			</div>
		</Tabs.Content>

				<Tabs.Content value="Sur place">
			<div class="flex flex-col md:flex-row items-center justify-center bg-gray-100 rounded-md p-4 gap-8">
				<img src={ImgSurPlace} alt="Logo Restauration" class="w-2/5">
				<div class="md:w-3/5">
				<h1 class="font-rock text-2xl m-2">ENTREE DU FESTIVAL</h1>
				<p class="text-justify m-1">
					Un contrôle des billets sera effectué à l’entrée du festival.
					<br>
					<br>
					Les portes du festival ouvrent le vendredi 6 septembre à 19h et le samedi 7 septembre à 17h. 
					<br>
					Les concerts commencent environ 1h après ces horaires.
				</p>
				</div>
			</div>
			<br />
		</Tabs.Content>

		<Tabs.Content value="Restauration">
			<div class="flex flex-col md:flex-row items-center justify-center bg-gray-100 rounded-md p-4 gap-8">
				<img src={ImgRestauration} alt="Logo Restauration" class="bg-black w-2/5">
				<div class="md:w-3/5">
					<h1 class="font-rock text-2xl m-2">Restauration sur place</h1>
					<p class="text-justify m-2">
						Sur le site du festival, nos bénévoles de la restauration se feront un plaisir de vous
						servir façon snacking !
					</p>
				</div>
			</div>
			<br />
		</Tabs.Content>

		<Tabs.Content value="Zone de nuit">
			<div class="flex flex-col md:flex-row items-center justify-center bg-gray-100 rounded-md p-4 gap-8">
				<img src={ImgCamping} alt="Logo Campings" class="bg-black w-2/5">
				<div class="md:w-3/5">
					<h1 class="font-rock text-2xl m-2">Zone de Nuit</h1>
					<p class="text-justify m-2">
						Une zone de nuit est à disposition des festivaliers qui souhaitent profiter de leur soirée en toute sécurité. L'accès au terrain est indiqué par des panneaux de signalétique depuis le parking
					</p>
				</div>
			</div>
			<br />
		</Tabs.Content>

		<Tabs.Content value="Eco-Festival">
			<div class="flex flex-col md:flex-row items-center justify-center bg-gray-100 rounded-md p-4 gap-8">
				
				<img src={ImgEcoFest} alt="festival ecolo" class="w-2/5">
				<div class="md:w-3/5">
				<p class="text-justify m-2">
					Nous apportons une attention toute particulière au respect du site et de l’environnement.
					<br/>
					Il s’agit en effet d’un immense champ qui voit habituellement les vaches d’une ferme biologique paître.
					<br/>
					<br/>
					Nous mettons tout en œuvre pour limiter l’impact environnemental en multipliant nos points de tri des déchets. Nous implantons également des toilettes sèches totalement gérées par une équipe de bénévoles.
					<br/>
					<br/>
					Nous privilégions les circuits courts. Nous veillons à impliquer au mieux nos artisans et commerçants locaux pour nos achats en matière de restauration et de bar que ce soit pour les festivaliers ou les artistes.
					<br/>
					<br/>
					Le site est également décoré avec des objets récupérés et détournés.
				</p>
				</div>
			</div>
			<br />
		</Tabs.Content>

		<Tabs.Content value="FAQ">
			<div class="flex flex-col justify-center bg-gray-100 rounded-md p-4 gap-8">
				<h1 class="font-rock text-2xl m-2">COMMENT ACHETER DES BILLETS POUR LE FESTIVAL ?</h1>
				<p class="text-justify m-2">Soit sur internet, soit dans certains commerces de La Grigonnais. Rendez-vous sur notre <a href="/Billetterie" class="text-red-500 hover:text-black">billetterie</a>.</p>
			</div>
			<br />
			<div class="flex flex-col justify-center bg-gray-100 rounded-md p-4 gap-8">
				<h1 class="font-rock text-2xl m-2">PUIS-JE ACHETER DES BILLETS LE JOUR DU FESTIVAL ?</h1>
				<p class="text-justify m-2">Dans le cas où le festival affiche complet, aucun ticket ne sera vendu sur place. Dans le cas contraire, des tickets seront en vente au guichet du festival.</p>
			</div>
			<br />
		</Tabs.Content>
	</Tabs.Root>
</section>
