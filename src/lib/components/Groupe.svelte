<script>
	// @ts-nocheck

	import Icon from '@iconify/svelte';

	export let Img = '';
	export let reseaus = [];
</script>

<div class="flex justify-center bg-gray-100 rounded-md p-4">
	<img src={Img} alt="" class="w-2/5" />
	<div lass="w-3/5">
		<slot name="name" />
		<slot name="style" />
		<ul>
			{#each reseaus as reseau}
				<li><slot name="reseau" {reseau} /></li>
			{/each}
		</ul>
		<slot name="description" />
	</div>
</div>
