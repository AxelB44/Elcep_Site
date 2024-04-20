<script>
	export let PartenaireImg = '';
	export let Name = '';

	let defaultImg = 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTY04kwTymJuvWhLtNvCzmAmhRWGNx86O5Yd5ZwcpZTJg&s'
</script>

<div class="flex flex-col items-center size-full">
	{#if PartenaireImg != ''}
	<img class="size-30 md:size-60" src={'../Partenaire/' + PartenaireImg} alt="Logo de {Name}" />
	{:else}
	<img class="size-30 md:size-60" src={defaultImg} alt="Logo de {Name}" />
	{/if}
	
	<h2 class="m-2 font-rock text-2xl text-center">{Name}</h2>
</div>
