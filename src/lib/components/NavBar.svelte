<script>
	import Logo from '../assets/ELCEP_logo_festival.png';
	import Icon from '@iconify/svelte';

	let togglesmenu = '-translate-y-full';
	let icon = 'ci:hamburger-lg';
	let MenuBtn = false;

	function togglesNav() {
		console.log(togglesmenu);
		if (togglesmenu == '-translate-y-full') {
			console.log(togglesmenu);
			togglesmenu = '';
			icon = 'akar-icons:cross';
			MenuBtn = true;
		} else {
			console.log(togglesmenu);
			togglesmenu = '-translate-y-full';
			icon = 'ci:hamburger-lg';
			MenuBtn = false;
		}

		console.log(togglesmenu);
	}
</script>

<header class="bg-neutral-900 z-50 fixed top-0 w-full">
	<nav
		class="bg-neutral-900 text-white max-w-screen-2xl mx-auto font-poppins p-6 flex items-center justify-between"
	>
		<a href="/"><img class="max-h-16" src={Logo} alt="" /></a>
		<button
			aria-label="toggle button"
			aria-expanded={MenuBtn}
			id="menu-btn"
			class="cursor-pointer w-7 md:hidden"
			on:click={togglesNav}
		>
			<Icon {icon} class="text-4xl" />
		</button>
		<ui
			id="toggles-menu"
			class="w-full absolute top-full left-0 {togglesmenu} -z-10 text-white bg-neutral-900 flex flex-col items-center md:static md:z-10 md:w-min md:transform-none md:border-none md:flex-row"
		>
			<li class="py-4 md:py-0 md:mr-6 hover:text-red-500">
				<a href="/" class="font-rock text-2xl">Accueil</a>
			</li>
			<li class="py-4 md:py-0 md:mr-6 hover:text-red-500">
				<a href="/Programation" class="font-rock text-2xl">Programmation</a>
			</li>
			<li class="py-4 md:py-0 md:mr-6 hover:text-red-500">
				<a href="/Billetterie" class="font-rock text-2xl">Billeterie</a>
			</li>
			<li class="py-4 md:py-0 md:mr-6 hover:text-red-500">
				<a href="/InfoPratique" class="font-rock text-2xl text-nowrap">Info Pratique</a>
			</li>
			<li class="py-4 md:py-0 md:mr-6 hover:text-red-500">
				<a href="/Archives" class="font-rock text-2xl">Archives</a>
			</li>
		</ui>
	</nav>
</header>
