<script>
	import PageLayout from '$lib/components/PageLayout.svelte';

	const features = [
		{
			icon: '🏛️',
			title: 'Governance Studies',
			description: 'Research on democratic governance and institutional development.'
		},
		{
			icon: '📊',
			title: 'Public Sector Reform',
			description: 'Analysis and recommendations for government efficiency improvements.'
		},
		{
			icon: '🌍',
			title: 'Development Policy',
			description: 'Strategies for sustainable economic and social development.'
		},
		{
			icon: '🤝',
			title: 'Public-Private Partnerships',
			description: 'Frameworks for collaboration between government and private sector.'
		},
		{
			icon: '📈',
			title: 'Economic Policy',
			description: 'Macroeconomic analysis and policy recommendations.'
		},
		{
			icon: '🗳️',
			title: 'Political Economy',
			description: 'Study of political systems and economic outcomes.'
		}
	];
</script>

<PageLayout
	title="Institute of Public Policy & Administration"
	subtitle="Shaping Policy for Better Governance"
	description="The Institute of Public Policy & Administration is dedicated to improving governance in Nigeria through rigorous research, policy analysis, and capacity building. We work with government agencies, civil society, and international organizations to develop evidence-based solutions to public challenges."
	heroImage="https://images.unsplash.com/photo-1555848962-6e79363ec58f?w=1200"
	{features}
	ctaText="Explore Public Policy Programs"
	ctaLink="/academics"
>
	<svelte:fragment slot="related-links">
		<a
			href="/institutions/oceanography"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			← Institute of Oceanography
		</a>
		<a
			href="/research"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			Research →
		</a>
		<a
			href="/"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			← Back to Home
		</a>
	</svelte:fragment>
</PageLayout>
