<script>
	import NavBar from '../lib/components/NavBar.svelte';
	import Footer from '../lib/components/Footer.svelte';
	import '../app.pcss';
</script>

<NavBar />
<main>
	<slot />
</main>
<Footer />

<style>
</style>
