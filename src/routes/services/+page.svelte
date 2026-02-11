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
			src="https://images.unsplash.com/photo-1517245386807-bb43f82c33c4?w=1200&h=600&fit=crop"
			alt="UNICAL Digital Services"
			class="w-full h-auto"
		/>
	</div>
</section>

<section class="md:flex gap-8 justify-center items-start px-6 py-12 mx-auto max-w-6xl">
	<div class="py-6 justify-center items-center flex mx-auto place-self-center">
		<h2 class="font-semibold text-3xl md:text-4xl">
			Comprehensive Digital Services for the<br class="hidden md:block" />UNICAL Community.
		</h2>
	</div>

	<div class="text-xl text-gray-500">
		Your gateway to seamless digital identity and access management at UNICAL. <br />
		We provide state-of-the-art solutions that ensure protected and intuitive <br />
		access throughout the campus. <br />

		From secure biometric verification to real-time communication platforms, <br />
		our services are designed to enhance your academic experience and keep <br />
		you connected with the university community.
	</div>
</section>

<section class="items-center justify-center mx-auto px-6 py-20 bg-gray-100/50">
	<div class="grid lg:grid-cols-2 gap-14 items-start max-w-7xl mx-auto">
		<!-- LEFT: Image Grid -->
		<div class="grid grid-cols-2 gap-8">
			<div class="flex flex-col gap-4">
				<img
					src="https://images.unsplash.com/photo-1550751827-4bd374c3f58b?w=600&h=400&fit=crop"
					alt="Biometric Security Technology"
					class="rounded-xl object-cover h-64 w-full"
				/>

				<img
					src="https://images.unsplash.com/photo-1454165804606-c3d57bc86b40?w=600&h=400&fit=crop"
					alt="Academic Management System"
					class="rounded-xl object-cover h-64 w-full"
				/>

				<img
					src="https://images.unsplash.com/photo-1611746872915-64382b5c76da?w=600&h=400&fit=crop"
					alt="University Communication Platform"
					class="rounded-xl object-cover h-64 w-full"
				/>
			</div>

			<div class="flex flex-col gap-4 mt-12">
				<img
					src="https://images.unsplash.com/photo-1573164713714-d95e436ab8d6?w=600&h=400&fit=crop"
					alt="Digital Campus Access"
					class="rounded-xl object-cover h-64 w-full"
				/>

				<img
					src="https://images.unsplash.com/photo-1531482615713-2afd69097998?w=600&h=400&fit=crop"
					alt="Student Online Services"
					class="rounded-xl object-cover h-64 w-full"
				/>

				<img
					src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f?w=600&h=400&fit=crop"
					alt="Campus Technology Hub"
					class="rounded-xl object-cover h-64 w-full"
				/>
			</div>
		</div>

		<!-- RIGHT: Content -->
		<div class="space-y-8">
			<h2 class="text-4xl lg:text-5xl font-semibold text-gray-900 leading-tight">
				UNICAL IDID<br />
				Digital Services.
			</h2>

			<p class="text-gray-600 text-lg sm:text-xl leading-relaxed">
				Leveraging state-of-the-art face verification, UNICAL IDID ensures protected and intuitive
				access throughout the campus. Secure your sensitive information and enjoy an efficient,
				seamless interaction.
			</p>

			<p class="text-gray-600 text-lg sm:text-xl leading-relaxed">
				Business and Academic Management System - A comprehensive platform for managing academic
				records, course registrations, and administrative processes with cutting-edge technology.
			</p>

			<p class="text-gray-600 text-lg sm:text-xl leading-relaxed">
				Stay connected with ease using UNICAL Messenger, your go-to communication platform for
				real-time updates, group discussions, and direct messaging within the university community.
			</p>

			<p class="text-gray-600 text-lg sm:text-xl leading-relaxed">
				We envision a future where your digital experience grows beyond expectations. Our dedication
				to innovation ensures we remain at the forefront, providing top-tier digital services.
			</p>

			<p class="text-gray-600 text-lg sm:text-xl leading-relaxed">
				Our modern resources, dedicated team, and focus on excellence ensure every interaction
				reflects quality, security, and a deep understanding of the UNICAL community needs.
			</p>
		</div>
	</div>
</section>

<!-- slider -->
<Slider />
