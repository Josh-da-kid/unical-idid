<script>
	import MenuIcon from '$lib/icons/MenuIcon.svelte';
	import { slide } from 'svelte/transition';
	import { Add } from 'carbon-icons-svelte';
	import Dropdown from './Dropdown.svelte';

	let isMobileMenuOpen = false;
	let expandedMobileSections = {};

	function toggleMobileMenu() {
		isMobileMenuOpen = !isMobileMenuOpen;
	}

	function toggleMobileSection(id) {
		expandedMobileSections[id] = !expandedMobileSections[id];
	}

	const academicsItems = [
		{ id: '0', text: 'Academics' }, // This will be unclickable trigger
		{
			id: '1',
			text: 'Faculties',
			children: [
				{ id: '1-1', text: 'Faculty of Arts', href: '/faculties/arts' },
				{ id: '1-2', text: 'Faculty of Science', href: '/faculties/science' },
				{ id: '1-3', text: 'Faculty of Law', href: '/faculties/law' },
				{ id: '1-4', text: 'Faculty of Engineering', href: '/faculties/engineering' },
				{ id: '1-5', text: 'Faculty of Education', href: '/faculties/education' }
			]
		},
		{
			id: '2',
			text: 'Colleges',
			children: [
				{ id: '2-1', text: 'College of Medical Sciences', href: '/colleges/medical-sciences' }
			]
		},
		{
			id: '3',
			text: 'Institutions',
			children: [
				{ id: '3-1', text: 'Institute of Education', href: '/institutions/education' },
				{ id: '3-2', text: 'Institute of Oceanography', href: '/institutions/oceanography' },
				{
					id: '3-3',
					text: 'Institute of Public Policy & Admin',
					href: '/institutions/public-policy'
				}
			]
		},
		{ id: '4', text: 'Research', href: '/research' }
	];
</script>

<header
	aria-label="UNICAL Hub"
	class="flex items-center justify-between px-3 sm:px-6 py-2 border-b border-gray-200"
>
	<div class="flex items-center">
		<img src="/unical-logo.jpeg" alt="" class="h-16 w-20 object-contain mr-4" />
		<a href="/" class="text-lg sm:text-3xl font-bold">
			<span class="font-bold text-blue-600">UNICAL IDID</span> Hub
		</a>
	</div>

	<!-- Mobile Menu Button -->
	<div class="lg:hidden">
		<button on:click={toggleMobileMenu} class="p-2 text-gray-600 focus:outline-none">
			<MenuIcon />
		</button>
	</div>

	<!-- Mobile Menu Overlay -->
	{#if isMobileMenuOpen}
		<div
			class="absolute left-0 top-16 z-50 flex w-full flex-col space-y-4 border-t border-gray-200 bg-white p-4 shadow-lg lg:hidden"
			transition:slide={{ duration: 300 }}
		>
			<a href="/" class="font-semibold text-gray-700" on:click={toggleMobileMenu}>Home</a>
			<a href="/about-us" class="font-semibold text-gray-700" on:click={toggleMobileMenu}
				>About Us</a
			>
			<a href="/services" class="font-semibold text-gray-700" on:click={toggleMobileMenu}
				>Services</a
			>

			<!-- Mobile Academics Accordion -->
			<div>
				<button
					class="flex w-full items-center justify-between font-semibold text-gray-700"
					on:click={() => toggleMobileSection('academics')}
				>
					Academics
					<i
						class="fa-solid fa-chevron-down transition-transform"
						class:rotate-180={expandedMobileSections['academics']}
					></i>
				</button>
				{#if expandedMobileSections['academics']}
					<div class="mt-2 space-y-2 border-l-2 border-gray-100 pl-4" transition:slide>
						{#each academicsItems.slice(1) as item}
							{#if item.children}
								<div>
									<button
										class="flex w-full items-center justify-between font-medium text-gray-600"
										on:click={() => toggleMobileSection(item.id)}
									>
										{item.text}
										<i
											class="fa-solid fa-chevron-down text-xs transition-transform"
											class:rotate-180={expandedMobileSections[item.id]}
										></i>
									</button>
									{#if expandedMobileSections[item.id]}
										<div class="mt-1 space-y-1 pl-4" transition:slide>
											{#each item.children as child}
												<a
													href={child.href}
													class="block py-1 text-sm text-gray-500"
													on:click={toggleMobileMenu}>{child.text}</a
												>
											{/each}
										</div>
									{/if}
								</div>
							{:else}
								<a
									href={item.href}
									class="block font-medium text-gray-600"
									on:click={toggleMobileMenu}>{item.text}</a
								>
							{/if}
						{/each}
					</div>
				{/if}
			</div>

			<a href="/news-events" class="font-semibold text-gray-700" on:click={toggleMobileMenu}
				>News & Events</a
			>
			<div class="flex flex-col space-y-3 border-t border-gray-200 pt-4">
				<a href="/login" class="font-semibold text-blue-600" on:click={toggleMobileMenu}>Login</a>
				<a
					href="/create-account"
					class="rounded bg-blue-600 py-2 text-center font-semibold text-white"
					on:click={toggleMobileMenu}>Create Account</a
				>
			</div>
		</div>
	{/if}

	<ul
		aria-label="Main navigation"
		class="hidden lg:flex space-x-6 text-lg font-semibold text-gray-600"
	>
		<li><a class="hover:text-blue-600" href="/">Home</a></li>
		<li><a class="hover:text-blue-600" href="/about-us">About Us</a></li>
		<li><a class="hover:text-blue-600" href="/services">Services</a></li>
		<!-- <li><a class="hover:text-blue-600" href="/administration">Administration</a></li> -->
		<Dropdown dropdownId="nav-1" selectedId="0" items={academicsItems} />
		<!-- <li><a class="hover:text-blue-600" href="/academics">Academics</a></li> -->
		<li><a class="hover:text-blue-600" href="/news-events">News & Events</a></li>
	</ul>

	<div class="font-semibold space-x-4 text-lg hidden lg:flex">
		<button class="text-blue-500 hover:scale-105 duration-300 transition-transform">Login</button>
		<button
			class="bg-blue-500 px-3 py-2 text-white hover:bg-blue-600 hover:scale-105 duration-300 transition-transform"
			>Create Account</button
		>
	</div>
</header>
