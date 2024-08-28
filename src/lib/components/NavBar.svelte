<script>
	import Logo from '../assets/ELCEP_logo_festival.png';
	import Icon from '@iconify/svelte';
	import Vache from '$lib/assets/illus_vache_rock.png';
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
		<a href="/" class="flex gap-3"
			><img class="max-h-16" src={Logo} alt="" /></a
		>
		<button
			aria-label="toggle button"
			aria-expanded={MenuBtn}
			id="menu-btn"
			class="cursor-pointer w-7 lg:hidden"
			on:click={togglesNav}
		>
			<Icon {icon} class="text-4xl" />
		</button>
		<ui
			id="toggles-menu"
			class="w-full absolute top-full left-0 lg:translate-y-full {togglesmenu} -z-10 text-white bg-neutral-900 flex flex-col items-center lg:static lg:z-10 lg:w-min lg:transform-none lg:border-none lg:flex-row"
		>
			<li class="py-4 lg:py-0 lg:mr-6 hover:text-black">
				<a
					href="/Billetterie"
					class="font-rock text-2xl px-5 bg-Bandeau bg-no-repeat bg-[length:9rem] bg-center"
					on:click={() => togglesNav()}>Billetterie</a
				>
			</li>
			<li class="py-4 lg:py-0 lg:mr-6 hover:text-red-500">
				<a href="/Boutique" class="font-rock text-2xl" on:click={() => togglesNav()}
					>Boutique</a
				>
			</li>
			<li class="py-4 lg:py-0 lg:mr-6 hover:text-red-500">
				<a href="/Programmation" class="font-rock text-2xl" on:click={() => togglesNav()}
					>Programmation</a
				>
			</li>
			<li class="py-4 lg:py-0 lg:mr-6 hover:text-red-500">
				<a href="/InfoPratique" class="font-rock text-2xl text-nowrap" on:click={() => togglesNav()}
					>Infos Pratiques</a
				>
			</li>
			<li class="py-4 lg:py-0 lg:mr-6 hover:text-red-500">
				<a href="/Presse" class="font-rock text-2xl text-nowrap" on:click={() => togglesNav()}
					>Presse</a
				>
			</li>
			<li class="py-4 lg:py-0 lg:mr-6 hover:text-red-500">
				<a href="/Archives" class="font-rock text-2xl" on:click={() => togglesNav()}>Archives</a>
			</li>
			
		</ui>
	</nav>
</header>
