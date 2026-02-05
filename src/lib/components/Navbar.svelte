<script>
	import { Header, HeaderNav, HeaderNavItem, OverflowMenu, OverflowMenuItem } from 'carbon-components-svelte';
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
		<OverflowMenu flipped>
	  <OverflowMenuItem text="Manage credentials" />
	  <OverflowMenuItem
		href="https://cloud.ibm.com/docs/api-gateway/"
		target="_blank"
		text="API documentation"
	  />
	  <OverflowMenuItem danger text="Delete service" />
	</OverflowMenu>

	</div>

	<ul
		aria-label="Main navigation"
		class="hidden lg:flex space-x-6 text-lg font-semibold text-gray-600"
	>
		<li><a class="hover:text-blue-600" href="#">Home</a></li>
		<li><a class="hover:text-blue-600" href="#">About Us</a></li>
		<li><a class="hover:text-blue-600" href="#">Services</a></li>
		<li><a class="hover:text-blue-600" href="#">Administration</a></li>
		<li><a class="hover:text-blue-600" href="#">Academics</a></li>
		<li><a class="hover:text-blue-600" href="#">News & Events</a></li>
	</ul>

	<div class="font-semibold space-x-4 text-lg hidden lg:flex">
		<button class="text-blue-500 hover:scale-105 duration-300 transition-transform">Login</button>
		<button
			class="bg-blue-500 px-3 py-2 text-white hover:bg-blue-600 hover:scale-105 duration-300 transition-transform"
			>Create Account</button
		>
	</div>
</header>
