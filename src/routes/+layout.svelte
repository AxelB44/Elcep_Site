<script>
	import NavBar from '../lib/components/NavBar.svelte';
	import Footer from '../lib/components/Footer.svelte';
	import '../app.pcss';
</script>

<NavBar />
<main class="mt-16">
	<slot />
</main>
<Footer />
