<script>
	import chantier from '$lib/images/Affiche.png';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<h1>EL CEP</h1>
	<span class="welcome">
		<picture>
			<source srcset={chantier} type="image/webp" />
			<img src={chantier} alt="Welcome" />
		</picture>
	</span>
</section>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Metal+Mania&display=swap');

	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}

	h1 {
		font-family: 'Metal Mania';
		font-size: 3.75rem;
		line-height: 1;
		font-weight: 700;
		letter-spacing: 0.25em;
	}
	.welcome {
		display: block;
		position: relative;
		width: 50%;
		height: 0;
		padding: 8px 0 calc(100% * 1241 / 1754) 0;
		margin-top: 1rem;
	}

	.welcome img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
	}
</style>
