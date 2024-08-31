<script>
	import Banniere from '../../lib/assets/Banniere.jpg';

	import * as Accordion from '$lib/components/ui/accordion';
	import * as Tabs from '$lib/components/ui/tabs';
	import ImgRestauration from '$lib/assets/RESTAURATION.png';
	import ImgSurPlace from '$lib/assets/Sur_Place.jpg';
	import ImgCamping from '$lib/assets/Zone_Nuit.jpg';
	import ImgEcoFest from '$lib/assets/EcoFest.png';
</script>

<section class="">
	<img src={Banniere} alt="" class="w-full" />
</section>

<section class="flex justify-center items-center">
	<Tabs.Root value="Localisation" class="w-11/12 md:w-5/6 flex flex-col m-4">
		<Tabs.List class="mb-4 h-auto block md:inline-flex" aria-orientation="horizontal">
			<Tabs.Trigger value="Localisation" class="font-rock text-xl md:text-3xl"
				>Localisation</Tabs.Trigger
			>
			<Tabs.Trigger value="Sur place" class="font-rock text-xl md:text-3xl">Sur place</Tabs.Trigger>
			<Tabs.Trigger value="Restauration" class="font-rock text-xl md:text-3xl"
				>Restauration</Tabs.Trigger
			>
			<Tabs.Trigger value="Zone de nuit" class="font-rock text-xl md:text-3xl"
				>Zone de nuit</Tabs.Trigger
			>
			<Tabs.Trigger value="Eco-Festival" class="font-rock text-xl md:text-3xl"
				>Eco-Festival</Tabs.Trigger
			>
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
					Aux abords de La Grigonnais, des panneaux de signalisation vous guideront vers le parking
					et l'entrée du festival.
					<br />
					Un grand parking est situé à proximité du site et est idéal pour ceux qui souhaitent repartir
					dans la soirée.
				</p>
			</div>
			<br />
			<div class="flex flex-col items-center justify-center bg-gray-100 rounded-md p-4 gap-8">
				<h1 class="font-rock text-2xl m-2">Transport en commun</h1>
				<p class="text-justify m-2">
					Les lignes Aléop 309 et 310 vous emmènent directement de Nantes à proximité du festival en
					à peine une heure, pour profiter pleinement de l'ambiance et des festivités.
				</p>
			</div>
		</Tabs.Content>

		<Tabs.Content value="Sur place">
			<div
				class="flex flex-col md:flex-row items-center justify-center bg-gray-100 rounded-md p-4 gap-8"
			>
				<img src={ImgSurPlace} alt="Logo Restauration" class="w-2/5" />
				<div class="md:w-3/5">
					<h1 class="font-rock text-2xl m-2">ENTREE DU FESTIVAL</h1>
					<p class="text-justify m-1">
						Un contrôle des billets sera effectué à l’entrée du festival.
						<br />
						<br />
						Les portes du festival ouvrent le vendredi 6 septembre à 19h et le samedi 7 septembre à 17h.
						<br />
						Les concerts commencent environ 1h après l'ouverture des portes.
					</p>
				</div>
			</div>
			<br />
		</Tabs.Content>

		<Tabs.Content value="Restauration">
			<div
				class="flex flex-col md:flex-row items-center justify-center bg-gray-100 rounded-md p-4 gap-8"
			>
				<img src={ImgRestauration} alt="Logo Restauration" class="bg-black w-2/5" />
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
			<div
				class="flex flex-col md:flex-row items-center justify-center bg-gray-100 rounded-md p-4 gap-8"
			>
				<img src={ImgCamping} alt="Logo Campings" class="bg-black w-2/5" />
				<div class="md:w-3/5">
					<h1 class="font-rock text-2xl m-2">Zone de Nuit</h1>
					<p class="text-justify m-2">
						Une zone de nuit est à disposition des festivaliers qui souhaitent profiter de leur
						soirée en toute sécurité. L'accès au terrain est indiqué par des panneaux de
						signalétique depuis le parking.
					</p>
				</div>
			</div>
			<br />
		</Tabs.Content>

		<Tabs.Content value="Eco-Festival">
			<div
				class="flex flex-col md:flex-row items-center justify-center bg-gray-100 rounded-md p-4 gap-8"
			>
				<img src={ImgEcoFest} alt="festival ecolo" class="w-2/5" />
				<div class="md:w-3/5">
					<p class="text-justify m-2">
						Nous apportons une attention toute particulière au respect du site et de
						l’environnement.
						<br />
						Il s’agit en effet d’un immense champ qui voit habituellement les vaches d’une ferme biologique
						paître.
						<br />
						<br />
						Nous mettons tout en œuvre pour limiter l’impact environnemental en multipliant nos points
						de tri des déchets. Nous implantons également des toilettes sèches totalement gérées par
						une équipe de bénévoles.
						<br />
						<br />
						Nous privilégions les circuits courts. Nous veillons à impliquer au mieux nos artisans et
						commerçants locaux pour nos achats en matière de restauration et de bar que ce soit pour
						les festivaliers ou les artistes.
						<br />
						<br />
						Le site est également décoré avec des objets récupérés et détournés.
					</p>
				</div>
			</div>
			<br />
		</Tabs.Content>

		<Tabs.Content value="FAQ">
			<Accordion.Root>
				<Accordion.Item value="item-1" class="bg-gray-100 rounded-md px-8">
					<Accordion.Trigger class="font-rock text-2xl m-2">
						COMMENT ACHETER DES BILLETS POUR LE FESTIVAL ?</Accordion.Trigger
					>
					<Accordion.Content class="text-justify m-2">
						Soit sur internet, soit dans certains commerces de La Grigonnais. Rendez-vous sur notre <a
							href="/Billetterie"
							class="text-red-500 hover:text-black">billetterie</a
						>.</Accordion.Content
					>
				</Accordion.Item>
				<br />
				<Accordion.Item value="item-2" class="bg-gray-100 rounded-md px-8">
					<Accordion.Trigger class="font-rock text-2xl m-2">
						PUIS-JE ACHETER DES BILLETS LE JOUR DU FESTIVAL ?</Accordion.Trigger
					>
					<Accordion.Content class="text-justify m-2">
						Dans le cas où le festival affiche complet, aucun ticket ne sera vendu sur place. Dans
						le cas contraire, des tickets seront en vente au guichet du festival.</Accordion.Content
					>
				</Accordion.Item>
				<br />
				<Accordion.Item value="item-3" class="bg-gray-100 rounded-md px-8">
					<Accordion.Trigger class="font-rock text-2xl m-2"
						>EST-CE QUE LES BILLETS SONT NOMINATIFS ?</Accordion.Trigger
					>
					<Accordion.Content class="text-justify m-2"
						>Les billets ne sont pas nominatifs.</Accordion.Content
					>
				</Accordion.Item>
				<br />
				<Accordion.Item value="item-4" class="bg-gray-100 rounded-md px-8">
					<Accordion.Trigger class="font-rock text-2xl m-2"
						>QUEL JUSTIFICATIF DOIS-JE APPORTER À L’ENTRÉE DU FESTIVAL ?</Accordion.Trigger
					>
					<Accordion.Content class="text-justify m-2"
						>La carte d’identité est obligatoire pour vérifier si tu es majeur. <br /> La carte d’étudiant
						et la carte de demandeur d’emploi te permettront d’avoir un tarif réduit.</Accordion.Content
					>
				</Accordion.Item>
				<br />
				<Accordion.Item value="item-5" class="bg-gray-100 rounded-md px-8">
					<Accordion.Trigger class="font-rock text-2xl m-2"
						>Y A T’IL UN ACCÈS PMR ?</Accordion.Trigger
					>
					<Accordion.Content class="text-justify m-2"
						>L’accès est accessible avec des roues tout terrains. Tout sera mis en place pour vous
						crée un accès.</Accordion.Content
					>
				</Accordion.Item>
				<br />
				<Accordion.Item value="item-6" class="bg-gray-100 rounded-md px-8">
					<Accordion.Trigger class="font-rock text-2xl m-2"
						>PUIS-JE SORTIR DU SITE DU FESTIVAL ?</Accordion.Trigger
					>
					<Accordion.Content class="text-justify m-2"
						>Les sorties seront autorisées avec une contremarque.</Accordion.Content
					>
				</Accordion.Item>
				<br />
				<Accordion.Item value="item-7" class="bg-gray-100 rounded-md px-8">
					<Accordion.Trigger class="font-rock text-2xl m-2"
						>QUELS SONT LES OBJETS INTERDITS SUR LE FESTIVAL ?</Accordion.Trigger
					>
					<Accordion.Content class="text-justify m-2"
						>
						Sont strictement interdits sur le site du festival :
						<br />
						Substances illicites (drogues, même douces), objets dangereux (tranchants & contondants),
						armes même factices, nourriture, feux d’artifice, boîtes de conserve et canettes, bouteilles
						et objets en verre, chaises (même pliantes), pointeurs laser, mégaphones & talkies, appareils
						de diffusion audio, animaux.
						<br />
						Il est interdit d’entrer avec de l’alcool sur le site du festival. Seules les gourdes à eau
						sont acceptées. De même dans un souci de respect de l’environnement, nous vous demandons
						de ne pas jeter vos mégots sur le sol.
						<br/>
						<br/>
						Le RECAP :
						<br/>
						<br/>
						<ul class="list-disc list-inside">
							<li>Bouteilles en verre / métallique / d’alcool</li>
							<li>Substances illicites</li>
							<li>Objets contondants</li>
							<li>Feux d’artifices</li>
							<li>Porte-voix</li>
							<li>Vélos / planches à roulettes / trottinette</li>
							<li>Ballons</li>
							<li>Pistolets à eau</li>
							<li>Parasols</li>
							<li>Glacières à flancs rigides</li>
							<li>Drones</li>
						</ul>
					</Accordion.Content>
				</Accordion.Item>
				<br />
				<Accordion.Item value="item-8" class="bg-gray-100 rounded-md px-8">
					<Accordion.Trigger class="font-rock text-2xl m-2">
						QUELS SONT LES DIFFÉRENTS MOYENS DE PAIEMENTS SUR LE FESTIVAL ?</Accordion.Trigger
					>
					<Accordion.Content class="text-justify m-2">
						Il sera possible de régler sur le festival en espèces ou en CB.</Accordion.Content
					>
				</Accordion.Item>
				<br />
				<Accordion.Item value="item-9" class="bg-gray-100 rounded-md px-8">
					<Accordion.Trigger class="font-rock text-2xl m-2">
						DES PROTECTIONS AUDITIVES SERONT-ELLES DISPONIBLES ?</Accordion.Trigger
					>
					<Accordion.Content class="text-justify m-2">
						Oui, les protections auditives sont disponibles sur le stand protection Entraid'addict.</Accordion.Content
					>
				</Accordion.Item>
				<br />
				<Accordion.Item value="item-10" class="bg-gray-100 rounded-md px-8">
					<Accordion.Trigger class="font-rock text-2xl m-2">
						EST-IL POSSIBLE DE PRENDRE DES PHOTOS SANS AVOIR DE PERMISSION PARTICULIÈRE ?</Accordion.Trigger
					>
					<Accordion.Content class="text-justify m-2">
						Il est en effet possible de prendre des photos sans permission à condition de ne pas utiliser de matériel professionnel.</Accordion.Content
					>
				</Accordion.Item>
				<br />
				<Accordion.Item value="item-11" class="bg-gray-100 rounded-md px-8">
					<Accordion.Trigger class="font-rock text-2xl m-2">
						LES ANIMAUX SONT-ILS AUTORISÉS DANS L’ENCEINTE DU FESTIVAL ?</Accordion.Trigger
					>
					<Accordion.Content class="text-justify m-2">
						Non les animaux ne sont pas autorisés.</Accordion.Content
					>
				</Accordion.Item>
				<br />
				<Accordion.Item value="item-12" class="bg-gray-100 rounded-md px-8">
					<Accordion.Trigger class="font-rock text-2xl m-2">
						QUELS SONT LES MOYENS MIS À DISPOSITION POUR COLLECTER MES DÉCHETS ?</Accordion.Trigger
					>
					<Accordion.Content class="text-justify m-2">
						Des poubelles de tri seront installées sur le site du festival ainsi que des cendriers seront à disposition. Le tri sera également guidé par vos valeurs et principes personnels.</Accordion.Content
					>
				</Accordion.Item>
			</Accordion.Root>
		</Tabs.Content>
	</Tabs.Root>
</section>
