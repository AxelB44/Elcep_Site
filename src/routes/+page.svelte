<script>
	import Counter from './Counter.svelte';
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
	import chantier from '$lib/images/en-chantier-1.png';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<h1> EL CEP </h1>
	<span class="welcome">
		<picture>
			<source srcset={chantier} type="image/webp" />
			<img src={chantier} alt="Welcome" />
		</picture>
	</span>
</section>

<style>

	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}

	h1 {
		font-family :"Roboto";
		font-size: 3.75rem;
		line-height: 1;
		font-weight: 700;
		letter-spacing: -0.025em;
	}
	.welcome {
		display: block;
		position: relative;
		width: 50%;
		height: 0;
		padding: 16px 0 calc(100% * 512 / 512) 0;
		margin-top:  5rem;
	}

	.welcome img {
		position: absolute;
		width: 100%;
		height: 50%;
		top: 0;
		display: block;
	}
</style>
