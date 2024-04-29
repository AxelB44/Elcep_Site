<script>
	import Banniere from '../../lib/assets/Banniere.jpg';
</script>

<!-- Baniere-->
<section class="">
	<img src={Banniere} alt="" class="w-full" />
</section>

<section class="flex flex-col p-12">
	<h1 class="text-center text-5xl font-rock mb-8">Billetterie</h1>
	<div class="flex md:flex-row flex-col justify-center items-center md:items-stretch md:gap-16">
		<div class="flex flex-col border rounded-xl w-5/6 lg:w-2/6 bg-gray-100 border-gray-100 p-4 m-4">
			<h1
				class="text-center font-rock text-3xl md:text-4xl mt-2 bg-Bandeau bg-no-repeat bg-[length:12rem] md:bg-[length:16rem] bg-center"
			>
				Vendredi
			</h1>
			<br />
			<br />
			<ul class="">
				<li class="flex justify-between md:text-2xl">
					<h3>Tarif unique</h3>
					<h3><strong>5 €</strong></h3>
				</li>
			</ul>

			<br />
			<button
				class="bg-neutral-900 hover:bg-red-500 rounded-full mt-auto ml-auto mr-auto p-4 font-rock text-3xl text-center text- text-white tracking-wider"
				>Acheter</button
			>
		</div>
		<div class="flex flex-col border rounded-xl w-5/6 lg:w-2/6 bg-gray-100 border-gray-100 p-4 m-4">
			<h1
				class="text-center font-rock text-3xl md:text-4xl mt-2 bg-Bandeau bg-no-repeat bg-[length:12rem] md:bg-[length:16rem] bg-center"
			>
				Samedi
			</h1>
			<br />
			<ul class="h-full">
				<li class="flex justify-between md:text-2xl">
					<h3>Plein Tarif</h3>
					<h3><strong>20 €</strong></h3>
				</li>
				<li class="flex justify-between md:text-2xl">
					<div>
						<h3>Tarif Réduit</h3>
						<h4>(étudiant et demandeur d'emploi)</h4>
					</div>
					<h3 class="text-nowrap"><strong>17 €</strong></h3>
				</li>
				<li class="flex justify-between md:text-2xl">
					<h3>Tarif - 12 ans</h3>
					<h3><strong>Gratuit</strong></h3>
				</li>
			</ul>

			<button
				class="bg-neutral-900 hover:bg-red-500 rounded-full mt-8 m-auto p-4 font-rock text-3xl text-center text-white tracking-wider"
				>Acheter</button
			>
		</div>
	</div>
	<br />
	<div
		class="flex flex-col border rounded-xl w-5/6 lg:w-2/6 bg-gray-100 border-gray-100 p-4 m-auto"
	>
		<h1
			class="text-center font-rock text-3xl md:text-4xl mt-2 bg-Bandeau bg-no-repeat bg-[length:12rem] md:bg-[length:16rem] bg-origin-border bg-bor bg-center"
		>
			Pass 2 jours
		</h1>
		<br />
		<br />
		<ul class="h-32">
			<li class="flex justify-between md:text-2xl">
				<h3>Tarif unique</h3>
				<h3><strong>20 €</strong></h3>
			</li>
		</ul>
		<button
			class="bg-neutral-900 hover:bg-red-500 rounded-full mt-8 m-auto p-4 font-rock text-3xl text-center text-white tracking-wider"
			>Acheter</button
		>
	</div>
</section>
