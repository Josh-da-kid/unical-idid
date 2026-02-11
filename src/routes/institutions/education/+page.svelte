<script>
	import PageLayout from '$lib/components/PageLayout.svelte';

	const features = [
		{
			icon: '📊',
			title: 'Educational Research',
			description: 'Cutting-edge research in teaching methods and learning outcomes.'
		},
		{
			icon: '👨‍🏫',
			title: 'Teacher Training',
			description: 'Professional development programs for educators at all levels.'
		},
		{
			icon: '📚',
			title: 'Curriculum Studies',
			description: 'Developing and evaluating educational curricula for Nigerian schools.'
		},
		{
			icon: '🔍',
			title: 'Policy Analysis',
			description: 'Research and analysis of educational policies and reforms.'
		},
		{
			icon: '📈',
			title: 'Assessment & Evaluation',
			description: 'Standardized testing and educational measurement services.'
		},
		{
			icon: '🤝',
			title: 'Community Outreach',
			description: 'Bringing quality education to underserved communities.'
		}
	];
</script>

<PageLayout
	title="Institute of Education"
	subtitle="Advancing Educational Excellence"
	description="The Institute of Education is UNICAL's center for educational research, policy development, and teacher professional development. We work to improve the quality of education across Nigeria through research, training, and community engagement."
	heroImage="https://images.unsplash.com/photo-1503676260728-1c00da094a0b?w=1200"
	{features}
	ctaText="Explore Education Programs"
	ctaLink="/academics"
>
	<svelte:fragment slot="related-links">
		<a
			href="/colleges/medical-sciences"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			← College of Medical Sciences
		</a>
		<a
			href="/institutions/oceanography"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			Institute of Oceanography →
		</a>
		<a
			href="/"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			← Back to Home
		</a>
	</svelte:fragment>
</PageLayout>
