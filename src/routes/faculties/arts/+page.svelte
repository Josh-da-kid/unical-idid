<script>
	import PageLayout from '$lib/components/PageLayout.svelte';

	const features = [
		{
			icon: '🎭',
			title: 'Performing Arts',
			description:
				'Theatre, Music, and Dance programs fostering creative expression and cultural preservation.'
		},
		{
			icon: '📚',
			title: 'Languages & Linguistics',
			description:
				'Comprehensive language studies including English, French, and indigenous Nigerian languages.'
		},
		{
			icon: '🏛️',
			title: 'History & International Studies',
			description:
				'Exploring global history, diplomacy, and international relations with African perspectives.'
		},
		{
			icon: '📖',
			title: 'Philosophy',
			description:
				'Critical thinking and ethical reasoning programs shaping future thought leaders.'
		},
		{
			icon: '🎨',
			title: 'Visual Arts',
			description: 'Fine arts, graphic design, and creative expression through various mediums.'
		},
		{
			icon: '📰',
			title: 'Mass Communication',
			description:
				'Journalism, broadcasting, and digital media training for the modern information age.'
		}
	];
</script>

<PageLayout
	title="Faculty of Arts"
	subtitle="Where Creativity Meets Critical Thinking"
	description="The Faculty of Arts at UNICAL is dedicated to nurturing creative minds and critical thinkers. Our programs blend traditional academic rigor with contemporary relevance, preparing students for careers in media, education, public service, and the creative industries."
	heroImage="https://images.unsplash.com/photo-1513364776144-60967b0f800f?w=1200"
	{features}
	ctaText="Explore Arts Programs"
	ctaLink="/academics"
>
	<svelte:fragment slot="related-links">
		<a
			href="/faculties/science"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			Faculty of Science →
		</a>
		<a
			href="/faculties/law"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			Faculty of Law →
		</a>
		<a
			href="/"
			class="px-6 py-3 bg-white rounded-lg shadow hover:shadow-md transition-shadow text-blue-600 font-medium"
		>
			← Back to Home
		</a>
	</svelte:fragment>
</PageLayout>
