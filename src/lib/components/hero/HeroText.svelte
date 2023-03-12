<script>
	import ButtonPrimary from '$lib/components/buttons/ButtonPrimary.svelte';
	import ButtonSecondary from '$lib/components/buttons/ButtonSecondary.svelte';
</script>

<div class="text-container">
	<div class="wrapper">
		<p class="pre-h">STEMMING, SERVICE, REPARASJONER & RENOVERING</p>
		<h1 class="h1">INNLANDET PIANO</h1>
		<p class="sub-h">
			Utfører alt av stemming, service, reparasjoner og renoveringer på flygler og pianoer over hele
			landet
		</p>

		<div class="buttons">
			<div class="button">
				<ButtonPrimary><a href="#">Ta kontakt</a></ButtonPrimary>
			</div>
			<div class="button">
				<ButtonSecondary><a href="#">Se presentasjon</a></ButtonSecondary>
			</div>
		</div>
	</div>
</div>

<style>
	.text-container {
		height: 86vh;
		display: grid;
		place-content: center;
		text-align: center;
	}

	.wrapper {
		width: 80%;
		margin: 0 auto;
		text-align: center;
		display: flex;
		flex-direction: column;
		align-items: center;
	}

	.pre-h {
		font-size: 31px;
		letter-spacing: 1.2px;
		font-weight: 300;
		margin-bottom: -16px;
	}

	h1 {
		color: var(--light);
	}

	.sub-h {
		font-size: 25px;
		width: 80%;
		margin-top: 16px;
		margin-bottom: 40px;
	}

	.buttons {
		display: flex;
		gap: 32px;
	}

	.button {
		width: 250px;
		height: 60px;
	}

	a {
		all: unset;
		font-size: 20px;
	}

	@media screen and (max-width: 1024px) {
		.wrapper {
			width: 100%;
		}

		.pre-h {
			font-size: 20px;
			letter-spacing: 1px;
			margin-bottom: -8px;
		}

		h1 {
			font-size: 61px;
			letter-spacing: 1.1px;
		}

		.sub-h {
			font-size: 16px;
			margin-top: 8px;
			margin-bottom: 24px;
			width: 70%;
		}

		.button {
			width: 180px;
			height: 50px;
		}

		a {
			font-size: 18px;
		}
	}

	@media screen and (max-width: 600px) {
		.wrapper {
			width: 100%;
		}

		.pre-h {
			font-size: 13px;
		}

		h1 {
			font-size: 39px;
			letter-spacing: 2px;
		}

		.sub-h {
			font-size: 14px;
			width: 305px;
		}

		.buttons {
			gap: 16px;
		}

		.button {
			width: 130px;
			height: 40px;
		}

		a {
			font-size: 16px;
		}
	}
</style>
