<script>
	export let AvatarImg = '';
	export let Name = '';
	export let Style = '';
</script>

<div class="flex flex-col items-center">
	<img class="size-28 m-2" src={AvatarImg} alt="Image du groupe {Name}" />
	<h2 class="m-2 font-rock">{Name}</h2>
	<h3 class="m-2">{Style}</h3>
</div>
