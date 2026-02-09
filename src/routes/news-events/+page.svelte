<script lang="ts">
	import Slider from '$lib/components/Slider.svelte';
	import { news } from '$lib/news-updates';
</script>

<section class="my-12 p-3">
	<h1 class="text-3xl lg:text-5xl font-bold text-center text-blue-600">Latest News and Events</h1>
	<p class="text-gray-500 text-xl lg:text-3xl font-semibold text-center mt-4">
		Stay informed with the latest developments, critical policy revisions, and <br /> important announcements
		impacting our community and the world beyond.
	</p>
</section>

<section class="bg-white py-14">
	<div class="max-w-6xl mx-auto px-4 lg:px-10">
		<!-- Grid -->
		<div class="grid md:grid-cols-2 gap-10">
			{#each news as post}
				<div
					class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition-shadow duration-300"
				>
					<div class="relative">
						<!-- Date badge -->
						<div
							class="absolute top-3 left-3 bg-white/50 rounded-md px-3 py-2 text-center text-gray-800"
						>
							<p class="text-2xl w-[60px]">{@html post.date}</p>
						</div>

						<!-- Image -->
						<img src={post.img} alt={post.heading} class="w-full h-56 object-cover" />
					</div>

					<!-- Text content -->
					<div class="p-6">
						<h4 class="font-semibold text-xl md:text-2xl text-gray-800 leading-snug mb-2">
							{post.heading}
						</h4>

						<p class="text-gray-700 text-lg sm:text-xl mb-4">
							{post.description}
						</p>

						<a
							href={`/info/${post.heading}`}
							class="text-blue-700 font-semibold underline text-lg sm:text-xl"
						>
							Read More
						</a>
					</div>
				</div>
			{/each}
		</div>

		<!-- Load More button -->
		<div class="flex justify-center mt-12">
			<button
				class="bg-blue-700 hover:bg-blue-800 text-white font-semibold text-lg px-6 py-3 rounded-lg transition-colors duration-200"
			>
				Load More News
			</button>
		</div>
	</div>
</section>

<!-- slider -->
<Slider />
