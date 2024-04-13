<script>
	export let PartenaireImg = '';
	export let Name = '';
</script>

<div class="flex flex-col items-center">
	<img class="size-60" src={PartenaireImg} alt="Logo de {Name}" />
	<h2 class="m-2 font-rock text-xl">{Name}</h2>
</div>
