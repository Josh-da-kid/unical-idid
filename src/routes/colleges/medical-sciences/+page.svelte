<script>
	import PageLayout from '$lib/components/PageLayout.svelte';

	const features = [
		{
			icon: '👨‍⚕️',
			title: 'Medicine & Surgery',
			description: 'Comprehensive MBBS program training future doctors with modern clinical skills.'
		},
		{
			icon: '🦷',
			title: 'Dentistry',
			description: 'Dental surgery and oral health sciences for comprehensive patient care.'
		},
		{
			icon: '💊',
			title: 'Pharmacy',
			description: 'Pharmaceutical sciences, drug development, and clinical pharmacy practice.'
		},
		{
			icon: '🧬',
			title: 'Medical Laboratory Science',
			description: 'Diagnostic laboratory techniques and biomedical research.'
		},
		{
			icon: '🏥',
			title: 'Nursing Science',
			description: 'Professional nursing education for diverse healthcare settings.'
		},
		{
			icon: '🧠',
			title: 'Basic Medical Sciences',
			description: 'Anatomy, physiology, biochemistry, and pathology fundamentals.'
		}
	];
</script>

<PageLayout
	title="College of Medical Sciences"
	subtitle="Excellence in Healthcare Education"
	description="The College of Medical Sciences at UNICAL is a premier institution for healthcare education and research. With state-of-the-art teaching hospitals and research facilities, we train the next generation of healthcare professionals who will serve Nigeria and beyond."
	heroImage="https://images.unsplash.com/photo-1576091160399-112ba8d25d1d?w=1200"
	{features}
	ctaText="Explore Medical Programs"
	ctaLink="/academics"
>
	<svelte:fragment slot="related-links">
		<a
			href="/faculties/education"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			← Faculty of Education
		</a>
		<a
			href="/institutions/education"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			Institute of Education →
		</a>
		<a
			href="/"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			← Back to Home
		</a>
	</svelte:fragment>
</PageLayout>
