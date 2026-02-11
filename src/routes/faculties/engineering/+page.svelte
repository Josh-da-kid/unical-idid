<script>
	import PageLayout from '$lib/components/PageLayout.svelte';

	const features = [
		{
			icon: '🏗️',
			title: 'Civil Engineering',
			description:
				'Infrastructure development, structural engineering, and construction management.'
		},
		{
			icon: '⚡',
			title: 'Electrical Engineering',
			description: 'Power systems, electronics, telecommunications, and renewable energy.'
		},
		{
			icon: '🔧',
			title: 'Mechanical Engineering',
			description: 'Thermodynamics, manufacturing, robotics, and automotive engineering.'
		},
		{
			icon: '🖥️',
			title: 'Computer Engineering',
			description: 'Hardware design, embedded systems, and computer architecture.'
		},
		{
			icon: '🌊',
			title: 'Marine Engineering',
			description: 'Ship design, offshore engineering, and coastal infrastructure.'
		},
		{
			icon: '🧪',
			title: 'Chemical Engineering',
			description: 'Process engineering, petrochemicals, and environmental engineering.'
		}
	];
</script>

<PageLayout
	title="Faculty of Engineering"
	subtitle="Innovation Through Engineering Excellence"
	description="The Faculty of Engineering equips students with the technical knowledge and practical skills needed to solve real-world problems. Our graduates are leaders in industry, research, and development across Nigeria and beyond."
	heroImage="https://images.unsplash.com/photo-1581092921461-eab62e97a782?w=1200"
	{features}
	ctaText="Explore Engineering Programs"
	ctaLink="/academics"
>
	<svelte:fragment slot="related-links">
		<a
			href="/faculties/law"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			← Faculty of Law
		</a>
		<a
			href="/faculties/education"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			Faculty of Education →
		</a>
		<a
			href="/"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			← Back to Home
		</a>
	</svelte:fragment>
</PageLayout>
