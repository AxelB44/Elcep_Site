<script>
	import * as Tabs from '$lib/components/ui/tabs';
	import Banniere from '../../lib/assets/Billeterie.jpg';
</script>

<!-- Baniere-->
<section class="">
	<img src={Banniere} alt="" class="w-full" />
</section>



<section class="flex flex-col p-12 h-full bg-gray-100">
	<h1 class="text-center text-5xl font-rock mb-8">Boutique</h1>
	<div class="flex w-full h-full">

		<!--
		<iframe
			title="Bouton Merch"
			id="haWidget"
			allowtransparency={true}
			src="https://www.helloasso.com/associations/association-culturelle-les-saltimbanques-de-la-grigonnais/boutiques/vente-de-textiles-el-cep-2024/widget-bouton"
			style="width: 100%; height: 70px; border: none;"
		></iframe>
	-->

		<iframe
			title="Bouton Merch"
			id="haWidget"
			allowtransparency={true}
			scrolling="yes"
			src="https://www.helloasso.com/associations/association-culturelle-les-saltimbanques-de-la-grigonnais/boutiques/vente-de-textiles-el-cep-2024-1/widget"
			class=" w-full h-[1900px]"
			height="100%" width="100%"
		></iframe>
		
	</div>
</section>
