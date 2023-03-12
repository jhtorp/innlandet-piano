<script>
	import HeroNav from '$lib/components/hero/HeroNav.svelte';
	import HeroText from '$lib/components/hero/HeroText.svelte';

	import backgroundVideo from '$lib/assets/innlandet-piano-bg-video.mp4';
	import stillPhoto from '$lib/assets/bg-loop-still.png';
</script>

<div class="container">
	<HeroNav />
	<HeroText />

	<img src={stillPhoto} alt="Bakgrunnsbilde" />

	<video class="video-bg" autoplay muted loop playsinline>
		<source src={backgroundVideo} type="video/mp4" />
	</video>
</div>

<style>
	.container {
		min-height: 100vh;
		position: relative;
		overflow: hidden;
		width: 100%;
	}

	.video-bg {
		width: 100%;
		min-height: 100%;
		position: absolute;
		top: 0;
		left: 0;
		object-fit: cover;
		z-index: -1;
	}

	img {
		display: none;
	}

	@media (max-width: 768px) {
		.video-bg {
			display: none;
		}

		img {
			display: block;
			width: 100%;
			min-height: 100%;
			position: absolute;
			top: 0;
			left: 0;
			object-fit: cover;
			z-index: -1;
		}
	}
</style>
