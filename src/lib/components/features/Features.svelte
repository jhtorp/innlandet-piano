<script>
	import flygelIcon from '$lib/assets/flygel.svg';
</script>

<div class="container">
	<div class="row row-1">
		<div class="card">
			<div class="header">
				<img src={flygelIcon} alt="Et ikon av et flygel" />
				<h3>Stemming</h3>
			</div>
			<p>
				Flygler og pianoer bør stemmes minst én gang i året uavhengig av bruk, men gjerne oftere.
				Produsentene anbefaler minst to ganger i året. Dette for å best mulig ivareta instrumentet,
				og bidra til at det holder seg over tid
			</p>
		</div>

		<div class="card">
			<div class="header">
				<img src={flygelIcon} alt="Et ikon av et flygel" />
				<h3>Service</h3>
			</div>
			<p>
				Et piano består av mange deler som skal fungere optimalt sammen. Dette kan man merke ved at
				for eksempel en eller flere toner låter ujevnt eller skarpt eller at tangenter oppleves
				forskjellige å spille på. Derfor trenger instrumentet også med jevne mellomrom en service
				hvor pianoteknikeren regulerer og intonerer instrumentet.
			</p>
		</div>
	</div>

	<div class="row row-2">
		<div class="card">
			<div class="header">
				<img src={flygelIcon} alt="Et ikon av et flygel" />
				<h3>Reparasjoner</h3>
			</div>
			<p>
				Tangenter eller pedaler som ikke virker, toner som ikke låter, knirk eller annen ulyd? Det
				aller meste på et flygel eller piano lar seg reparere! For å forebygge slike problemer
				anbefaler Innlandet Piano å få installert et eget klimaanlegg for å bevare kvaliteten til
				instrumentet og holde stemmingen bedre.
			</p>
		</div>

		<div class="card">
			<div class="header">
				<img src={flygelIcon} alt="Et ikon av et flygel" />
				<h3>Renovering</h3>
			</div>
			<p>
				Av og til kan det være nødvendig med en større gjennomgang av flygelet eller pianoet for å
				hjelpe det tilbake til et bra instrument! Mekaniske deler kan være utslitt og må byttes,
				eller det trenger en større gjennomgang med justeringer.
			</p>
		</div>
	</div>
</div>

<style>
	.container {
		max-width: 400px;
		margin: 64px auto 64px auto;
		display: flex;
		flex-direction: column;
		gap: 64px;
	}

	.header {
		display: flex;
		align-items: center;
		gap: 16px;
	}

	img {
		width: 35px;
		height: 35px;
	}

	h3 {
		font-size: 20px;
		font-weight: bold;
	}

	p {
		font-size: 16px;
		color: var(--dark);
		margin-top: 8px;
	}

	.row {
		display: flex;
		flex-direction: column;
		gap: 48px;
	}

	@media screen and (min-width: 768px) {
		.container {
			max-width: 600px;
		}
	}

	@media screen and (min-width: 1024px) {
		.container {
			min-width: 960px;
			max-width: 1440px;
			margin: 128px 48px;
		}

		.row {
			display: flex;
			flex-direction: row;
			justify-content: space-around;
		}

		.card {
			flex: 1;
		}
	}

	@media screen and (min-width: 1276px) {
		.row {
			gap: 128px;
		}
	}

	@media screen and (min-width: 1500px) {
		.container {
			margin: 128px auto;
		}
	}
</style>
