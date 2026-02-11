<script lang="ts">
	export let title: string;
	export let subtitle: string = '';
	export let description: string = '';
	export let heroImage: string = '/images.jpeg';
	export let features: { icon: string; title: string; description: string }[] = [];
	export let ctaText: string = 'Learn More';
	export let ctaLink: string = '#';
</script>

<!-- Hero Section -->
<section
	class="relative h-[50vh] min-h-[400px] bg-cover bg-center"
	style="background-image: url('{heroImage}');"
>
	<div class="absolute inset-0 bg-gradient-to-r from-blue-900/80 to-blue-600/60"></div>
	<div class="relative z-10 flex h-full items-center justify-center px-6">
		<div class="max-w-4xl text-center text-white space-y-4">
			<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight">{title}</h1>
			{#if subtitle}
				<p class="text-xl md:text-2xl text-blue-100">{subtitle}</p>
			{/if}
		</div>
	</div>
</section>

<!-- Description Section -->
{#if description}
	<section class="py-16 px-6 bg-white">
		<div class="max-w-4xl mx-auto text-center space-y-6">
			<p class="text-xl md:text-2xl text-gray-600 leading-relaxed">{description}</p>
		</div>
	</section>
{/if}

<!-- Features Grid -->
{#if features.length > 0}
	<section class="py-16 px-6 bg-gray-50">
		<div class="max-w-7xl mx-auto">
			<div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
				{#each features as feature}
					<div class="bg-white p-8 rounded-lg shadow-md hover:shadow-xl transition-shadow">
						<div class="text-4xl mb-4">{feature.icon}</div>
						<h3 class="text-xl font-semibold mb-3 text-gray-900">{feature.title}</h3>
						<p class="text-gray-600">{feature.description}</p>
					</div>
				{/each}
			</div>
		</div>
	</section>
{/if}

<!-- CTA Section -->
<section class="py-16 px-6 bg-blue-600">
	<div class="max-w-4xl mx-auto text-center space-y-6">
		<h2 class="text-3xl md:text-4xl font-bold text-white">Ready to Get Started?</h2>
		<p class="text-xl text-blue-100">
			Explore more about {title} and discover how we can help you achieve your goals.
		</p>
		<a
			href={ctaLink}
			class="inline-block bg-white text-blue-600 px-8 py-4 rounded-lg font-semibold text-lg hover:bg-gray-100 transition-colors"
		>
			{ctaText}
		</a>
	</div>
</section>

<!-- Related Links -->
<section class="py-12 px-6 bg-gray-100">
	<div class="max-w-7xl mx-auto">
		<h3 class="text-2xl font-semibold mb-8 text-center text-gray-900">Explore More</h3>
		<div class="flex flex-wrap justify-center gap-4">
			<slot name="related-links">
				<a
					href="/"
					class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
				>
					← Back to Home
				</a>
			</slot>
		</div>
	</div>
</section>
