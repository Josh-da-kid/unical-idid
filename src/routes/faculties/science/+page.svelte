<script>
	import PageLayout from '$lib/components/PageLayout.svelte';

	const features = [
		{
			icon: '🧬',
			title: 'Biological Sciences',
			description:
				'Cutting-edge research in microbiology, genetics, biotechnology, and environmental biology.'
		},
		{
			icon: '⚗️',
			title: 'Chemistry',
			description:
				'Comprehensive programs in organic, inorganic, physical, and analytical chemistry.'
		},
		{
			icon: '🌍',
			title: 'Earth Sciences',
			description:
				'Geology, geophysics, and environmental science for sustainable resource management.'
		},
		{
			icon: '🧮',
			title: 'Mathematics',
			description: 'Pure and applied mathematics, statistics, and computational mathematics.'
		},
		{
			icon: '🔬',
			title: 'Physics',
			description: 'From theoretical physics to applied physics and renewable energy research.'
		},
		{
			icon: '🌊',
			title: 'Oceanography',
			description: 'Marine science research leveraging our proximity to the Atlantic Ocean.'
		}
	];
</script>

<PageLayout
	title="Faculty of Science"
	subtitle="Pioneering Research and Discovery"
	description="The Faculty of Science is committed to excellence in scientific research and education. With state-of-the-art laboratories and research facilities, we prepare students for careers in research, industry, healthcare, and environmental management."
	heroImage="https://images.unsplash.com/photo-1532094349884-543bc11b234d?w=1200"
	{features}
	ctaText="Explore Science Programs"
	ctaLink="/academics"
>
	<svelte:fragment slot="related-links">
		<a
			href="/faculties/arts"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			← Faculty of Arts
		</a>
		<a
			href="/faculties/engineering"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			Faculty of Engineering →
		</a>
		<a
			href="/"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			← Back to Home
		</a>
	</svelte:fragment>
</PageLayout>
