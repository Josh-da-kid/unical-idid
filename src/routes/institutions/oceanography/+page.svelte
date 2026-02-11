<script>
	import PageLayout from '$lib/components/PageLayout.svelte';

	const features = [
		{
			icon: '🌊',
			title: 'Marine Biology',
			description:
				"Study of marine ecosystems, biodiversity, and aquatic life along Nigeria's coast."
		},
		{
			icon: '🐟',
			title: 'Fisheries Science',
			description: 'Sustainable fisheries management and aquaculture development.'
		},
		{
			icon: '🌡️',
			title: 'Ocean Climate Research',
			description: 'Studying climate change impacts on marine environments.'
		},
		{
			icon: '🛢️',
			title: 'Marine Geology',
			description: 'Offshore resource exploration and coastal geology studies.'
		},
		{
			icon: '⚗️',
			title: 'Marine Chemistry',
			description: 'Chemical oceanography and marine pollution monitoring.'
		},
		{
			icon: '📊',
			title: 'Ocean Data Science',
			description: 'Big data analytics for ocean and coastal management.'
		}
	];
</script>

<PageLayout
	title="Institute of Oceanography"
	subtitle="Exploring Nigeria's Marine Frontier"
	description="Located in Calabar, the Institute of Oceanography leverages our proximity to the Atlantic Ocean to conduct cutting-edge marine research. We address critical issues in fisheries, climate change, and marine resource management for sustainable development."
	heroImage="https://images.unsplash.com/photo-1551244072-5d12893278ab?w=1200"
	{features}
	ctaText="Explore Oceanography Programs"
	ctaLink="/academics"
>
	<svelte:fragment slot="related-links">
		<a
			href="/institutions/education"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			← Institute of Education
		</a>
		<a
			href="/institutions/public-policy"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			Institute of Public Policy →
		</a>
		<a
			href="/"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			← Back to Home
		</a>
	</svelte:fragment>
</PageLayout>
