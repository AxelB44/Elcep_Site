<script>
	// @ts-nocheck

	import Icon from '@iconify/svelte';

	export let Img = '';
	export let Reseaux = [];
	export let order = 'order-none';
</script>

<div class="flex md:flex-row flex-col items-center justify-center bg-gray-100 rounded-md p-4 gap-8">
	<img src={'../Artiste/' + Img} alt="" class="md:w-2/5 {order} rounded-sm" />
	<div class="md:w-3/5">
		<slot name="name" />
		<ul class="flex text-4xl ml-4 text-neutral-700">
			{#each Reseaux as reseau}
				<li class="mr-8 hover:text-red-500">
					<a href={reseau.Link} target="_blank">
						<Icon icon={reseau.Icon} />
					</a>
				</li>
			{/each}
		</ul>
		<slot name="description" />
	</div>
</div>
