<script>
	import '../styles.css';

	import Hero from '$lib/components/hero/Hero.svelte';
	import Features from '$lib/components/features/Features.svelte';
</script>

<section class="hero-section">
	<Hero />
</section>

<section class="features-section">
	<Features />
</section>

<style>
	.features-section {
		padding-inline: 8px;
	}

	@media screen and (min-width: 1024px) {
		.features-section {
			padding-inline: 0;
		}
	}
</style>
