<script>
	export let AvatarImg = '';
	export let Name = '';
</script>

<div class="flex flex-col items-center">
	<img class="size-28 m-2 rounded-full" src={AvatarImg} alt="Image du groupe {Name}" />
	<h2 class="m-2 text-2xl font-rock text-center">{Name}</h2>
</div>
