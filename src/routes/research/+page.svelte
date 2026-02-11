<script>
	import PageLayout from '$lib/components/PageLayout.svelte';

	const features = [
		{
			icon: '🔬',
			title: 'Fundamental Research',
			description: 'Basic science research expanding the frontiers of human knowledge.'
		},
		{
			icon: '💡',
			title: 'Applied Research',
			description: 'Solving real-world problems through innovative research solutions.'
		},
		{
			icon: '🤝',
			title: 'Collaborative Projects',
			description: 'Partnerships with industry, government, and international institutions.'
		},
		{
			icon: '📚',
			title: 'Research Publications',
			description: 'Contributing to global knowledge through peer-reviewed publications.'
		},
		{
			icon: '🎓',
			title: 'Postgraduate Training',
			description: 'Masters and PhD programs for future researchers.'
		},
		{
			icon: '🏆',
			title: 'Research Grants',
			description: 'Securing funding for groundbreaking research initiatives.'
		}
	];
</script>

<PageLayout
	title="Research at UNICAL"
	subtitle="Advancing Knowledge, Transforming Lives"
	description="Research is at the heart of UNICAL's mission. Our researchers tackle critical challenges facing Nigeria and the world, from healthcare and climate change to governance and technology. We foster a culture of innovation and excellence that produces impactful results."
	heroImage="https://images.unsplash.com/photo-1532094349884-543bc11b234d?w=1200"
	{features}
	ctaText="Explore Research Opportunities"
	ctaLink="/academics"
>
	<svelte:fragment slot="related-links">
		<a
			href="/institutions/public-policy"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			← Institute of Public Policy
		</a>
		<a
			href="/services"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			Services →
		</a>
		<a
			href="/"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			← Back to Home
		</a>
	</svelte:fragment>
</PageLayout>
