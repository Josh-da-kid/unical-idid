<script>
	import PageLayout from '$lib/components/PageLayout.svelte';

	const features = [
		{
			icon: '📚',
			title: 'Educational Administration',
			description: 'Leadership and management skills for educational institutions.'
		},
		{
			icon: '🧠',
			title: 'Educational Psychology',
			description: 'Understanding learning processes and student development.'
		},
		{
			icon: '📖',
			title: 'Curriculum Development',
			description: 'Designing effective educational programs and materials.'
		},
		{
			icon: '👨‍🏫',
			title: 'Teacher Education',
			description: 'Preparing the next generation of qualified educators.'
		},
		{
			icon: '🎓',
			title: 'Guidance & Counseling',
			description: 'Supporting student wellbeing and career development.'
		},
		{
			icon: '🔬',
			title: 'Science Education',
			description: 'Training teachers in STEM subjects and laboratory management.'
		}
	];
</script>

<PageLayout
	title="Faculty of Education"
	subtitle="Shaping the Future of Learning"
	description="The Faculty of Education is committed to producing world-class educators and educational leaders. We combine pedagogical theory with practical experience to prepare graduates who can transform Nigeria's educational landscape."
	heroImage="https://images.unsplash.com/photo-1524178232363-1fb2b075b655?w=1200"
	{features}
	ctaText="Explore Education Programs"
	ctaLink="/academics"
>
	<svelte:fragment slot="related-links">
		<a
			href="/faculties/engineering"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			← Faculty of Engineering
		</a>
		<a
			href="/colleges/medical-sciences"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			College of Medical Sciences →
		</a>
		<a
			href="/"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			← Back to Home
		</a>
	</svelte:fragment>
</PageLayout>
