<script>
	import MenuIcon from '$lib/icons/MenuIcon.svelte';
	import {
		Header,
		HeaderNav,
		HeaderNavItem,
		OverflowMenu,
		OverflowMenuItem
	} from 'carbon-components-svelte';
	import { Add } from 'carbon-icons-svelte';
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

	<div class="lg:hidden">
		<OverflowMenu flipped icon={MenuIcon}>
			<OverflowMenuItem href="#" text="Home" />
			<OverflowMenuItem href="/about-us" text="About Us" />
			<OverflowMenuItem href="/services" text="Services" />
			<OverflowMenuItem href="/administration" text="Administration" />
			<OverflowMenuItem href="/academics" text="Academics" />
			<OverflowMenuItem href="/news-events" text="News & Events" />
			<OverflowMenuItem href="/login" text="Login" />
			<OverflowMenuItem href="/create-account" text="Create Account" />
		</OverflowMenu>
	</div>

	<ul
		aria-label="Main navigation"
		class="hidden lg:flex space-x-6 text-lg font-semibold text-gray-600"
	>
		<li><a class="hover:text-blue-600" href="/">Home</a></li>
		<li><a class="hover:text-blue-600" href="/about-us">About Us</a></li>
		<li><a class="hover:text-blue-600" href="/services">Services</a></li>
		<li><a class="hover:text-blue-600" href="/administration">Administration</a></li>
		<li><a class="hover:text-blue-600" href="/academics">Academics</a></li>
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
