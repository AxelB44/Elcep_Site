<script>
	import Baniere from '../../lib/assets/Banniere.jpg';
</script>

<!-- Baniere-->
<section class="">
	<img src={Baniere} alt="" class="w-full" />
</section>

<section class="flex flex-col p-12">
	<h1 class="text-center text-5xl font-rock mb-8">Billetterie</h1>
	<div class="flex md:flex-row flex-col justify-around items-center">
		<div class="flex flex-col border rounded-xl w-4/6 lg:w-2/6 bg-gray-100 border-gray-100 p-4 m-4">
			<h1 class="text-center font-rock text-4xl mt-2">Vendredi</h1>
			<br />
			<ul class="h-72">
				<li class="flex justify-between text-2xl">
					<h3>Tarif unique</h3>
					<h3>5 €</h3>
				</li>
			</ul>
		</div>
		<div class="flex flex-col border rounded-xl w-4/6 lg:w-2/6 bg-gray-100 border-gray-100 p-4 m-4">
			<h1 class="text-center font-rock text-4xl mt-2">Samedi</h1>
			<br />
			<ul class="h-72">
				<li class="flex justify-between text-2xl">
					<h3>Plein Tarif</h3>
					<h3>20 €</h3>
				</li>
				<li class="flex justify-between text-2xl">
					<div>
						<h3>Tarif Réduit</h3>
						<h4>(étudiant et demandeur d'emploi)</h4>
					</div>
					<h3>17 €</h3>
				</li>
				<li class="flex justify-between text-2xl">
					<h3>Tarif - 12 ans</h3>
					<h3>Gratuit</h3>
				</li>
			</ul>
		</div>
	</div>
	<br>
	<div class="flex flex-col border rounded-xl w-4/6 lg:w-5/6 bg-gray-100 border-gray-100 p-4 m-auto">
			<h1 class="text-center font-rock text-4xl mt-2">Pass 2 jours</h1>
			<br />
			<ul class="h-72">
				<li class="flex justify-between text-2xl">
					<h3>Tarif unique</h3>
					<h3>20 €</h3>
				</li>
			</ul>
		</div>
</section>
