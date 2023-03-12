<script>
	import '../styles.css';

	import Hero from '$lib/components/hero/Hero.svelte';
	import Features from '$lib/components/features/Features.svelte';
	import Presentation from '$lib/components/presentation/Presentation.svelte';
	import Recommendations from '$lib/components/recommendations/Recommendations.svelte';
</script>

<section class="hero-section">
	<Hero />
</section>
<main>
	<section class="features-section">
		<Features />
	</section>

	<section class="presentation-container">
		<Presentation />
	</section>

	<section class="recommendations-container">
		<Recommendations />
	</section>
</main>

<style>
	.features-section,
	.recommendations-container {
		padding-inline: 5%;
	}

	@media screen and (min-width: 1024px) {
		.features-section {
			padding-inline: 0;
		}
	}
</style>
