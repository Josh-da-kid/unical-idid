<script>
	import PageLayout from '$lib/components/PageLayout.svelte';

	const features = [
		{
			icon: '⚖️',
			title: 'Nigerian Legal System',
			description:
				'Comprehensive study of Nigerian constitutional, criminal, and civil law frameworks.'
		},
		{
			icon: '📜',
			title: 'International Law',
			description: 'Global legal systems, human rights law, and international dispute resolution.'
		},
		{
			icon: '🏢',
			title: 'Commercial Law',
			description: 'Business law, corporate governance, and commercial transactions expertise.'
		},
		{
			icon: '🌿',
			title: 'Environmental Law',
			description: 'Legal frameworks for environmental protection and sustainable development.'
		},
		{
			icon: '👨‍👩‍👧',
			title: 'Family Law',
			description: 'Marriage, divorce, child custody, and inheritance law in Nigeria.'
		},
		{
			icon: '📚',
			title: 'Jurisprudence',
			description: 'Legal theory, philosophy of law, and critical legal studies.'
		}
	];
</script>

<PageLayout
	title="Faculty of Law"
	subtitle="Shaping Future Legal Minds"
	description="The Faculty of Law at UNICAL is renowned for producing exceptional legal practitioners and scholars. Our rigorous curriculum combines theoretical knowledge with practical skills, preparing students for successful careers in the judiciary, private practice, and public service."
	heroImage="https://images.unsplash.com/photo-1589829545856-d10d557cf95f?w=1200"
	{features}
	ctaText="Explore Law Programs"
	ctaLink="/academics"
>
	<svelte:fragment slot="related-links">
		<a
			href="/faculties/science"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			← Faculty of Science
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
