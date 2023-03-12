<script>
	import logo from '$lib/assets/logo.svg';
	import ButtonSecondary from '$lib/components/buttons/ButtonSecondary.svelte';
</script>

<header>
	<img src={logo} alt="Logoen til Innlandet Piano som ser ut som et flygel" />
	<div class="button">
		<ButtonSecondary><a href="#">Ta kontakt</a></ButtonSecondary>
	</div>
</header>

<style>
	header {
		margin: 0 auto;
		display: flex;
		justify-content: space-between;
		align-items: center;
		max-width: 1440px;
		min-height: 8vh;
	}

	img {
		width: 50px;
		height: 51px;
	}

	.button {
		width: 140px;
		height: 45px;
	}

	a {
		all: unset;
		font-size: 18px;
	}
	@media screen and (max-width: 1440px) {
		header {
			margin: 0 48px;
		}
	}

	@media screen and (max-width: 1024px) {
		.button {
			width: 120px;
			height: 40px;
		}

		a {
			font-size: 16px;
		}

		img {
			width: 40px;
			height: 41px;
		}
	}

	@media screen and (max-width: 600px) {
		header {
			margin: 0 16px;
		}
	}
</style>
