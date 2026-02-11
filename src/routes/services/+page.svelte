<script>
	import Slider from '$lib/components/Slider.svelte';
	import { Button } from 'carbon-components-svelte';
</script>

<section class="flex flex-col items-center justify-center space-y-6 px-6 py-6 mx-auto max-w-6xl">
	<h1 class="text-3xl lg:text-5xl font-bold text-center text-blue-600">Our Services</h1>
	<p class="text-lg sm:text-xl lg:text-2xl text-center mt-4 font-semibold text-gray-500">
		UNICAL Hub provides cutting-edge digital services designed to empower students,<br /> faculty,
		and staff with seamless access to essential <br /> campus resources and services.
	</p>
	<div class="w-full items-center flex justify-center">
		<img
			src="https://www.shutterstock.com/image-photo/teamwork-team-community-holding-hands-600nw-2363785805.jpg"
			alt="UNICAL Services"
			class="w-full h-auto"
		/>
	</div>
</section>

<section class="md:flex gap-8 justify-center items-start px-6 py-12 mx-auto max-w-6xl">
	<div class="py-6 justify-center items-center flex mx-auto place-self-center w-full">
		<h2 class="font-semibold text-3xl md:text-4xl">
			Comprehensive Digital Services for the<br class="hidden md:block" />UNICAL Community.
		</h2>
	</div>

	<div
		class="text-start text-lg sm:text-xl text-gray-500 flex flex-col gap-4 justify-center mx-auto place-self-center"
	>
		<div>Your gateway to seamless digital identity and access management at UNICAL.</div>

		<div>
			We provide state-of-the-art solutions that ensure protected and intuitive access throughout
			the campus.
		</div>

		<div>
			From secure biometric verification to real-time communication platforms, our services are
			designed to enhance your academic experience and keep you connected with the university
			community.
		</div>
	</div>
</section>

<section class="items-center justify-center mx-auto px-6 py-20 bg-gray-100/50">
	<div class="max-w-7xl mx-auto space-y-16">
		<h2 class="text-4xl lg:text-5xl font-semibold text-gray-900 leading-tight text-center">
			UNICAL IDID Digital Services.
		</h2>

		<!-- Service 1: Identity & Biometric -->
		<div class="grid lg:grid-cols-2 gap-14 items-center">
			<div class="order-2 lg:order-1 space-y-6">
				<h3 class="text-3xl font-semibold text-blue-600">Identity & Biometric</h3>
				<p class="text-gray-600 text-lg sm:text-xl leading-relaxed">
					Leveraging state-of-the-art face verification, UNICAL IDID <br />
					ensures protected and intuitive access throughout the campus. <br />
					Secure your sensitive information and enjoy an efficient, seamless <br />
					interaction.
				</p>
				<Button href="/identify-biometric">Access</Button>
			</div>
			<div class="order-1 lg:order-2">
				<img
					src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRBFtPogRcJSPmgzirUEOGeNfb7_CoFIus0qg&s"
					alt="Identity and Biometric Service"
					class="rounded-xl object-cover h-80 w-full"
				/>
			</div>
		</div>

		<!-- Service 2: BAAMS -->
		<div class="grid lg:grid-cols-2 gap-14 items-center">
			<div>
				<img
					src="https://media.istockphoto.com/id/1220629405/photo/man-holding-light-bulbs-ideas-of-new-ideas-with-innovative-technology-and-creativity.jpg?s=612x612&w=0&k=20&c=QtFDsJUkcTEFmJ94YliS9UjtobZM-mBdR2Wue4sL6qc="
					alt="BAAMS Service"
					class="rounded-xl object-cover h-80 w-full"
				/>
			</div>
			<div class="space-y-6">
				<h3 class="text-3xl font-semibold text-blue-600">BAAMS</h3>
				<p class="text-gray-600 text-lg sm:text-xl leading-relaxed">
					Business and Academic Management System - A comprehensive <br />
					platform for managing academic records, course registrations, <br />
					and administrative processes with cutting-edge technology.
				</p>
				<Button href="/baams">Access</Button>
			</div>
		</div>

		<!-- Service 3: UNICAL Messenger -->
		<div class="grid lg:grid-cols-2 gap-14 items-center">
			<div class="order-2 lg:order-1 space-y-6">
				<h3 class="text-3xl font-semibold text-blue-600">UNICAL Messenger</h3>
				<p class="text-gray-600 text-lg sm:text-xl leading-relaxed">
					Stay connected with ease using UNICAL Messenger, your go-to <br />
					communication platform for real-time updates, group discussions, <br />
					and direct messaging within the university community.
				</p>
				<Button href="/unical-messenger">Access</Button>
			</div>
			<div class="order-1 lg:order-2">
				<img
					src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR9I9WoATXpTSOa2A6k2jPMKiRT1rDq5smFug&s"
					alt="UNICAL Messenger"
					class="rounded-xl object-cover h-80 w-full"
				/>
			</div>
		</div>
	</div>
</section>

<!-- slider -->
<Slider />
