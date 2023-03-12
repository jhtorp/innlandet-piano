<script>
	import quote from '$lib/assets/quote.svg';
	import avatarHaavard from '$lib/assets/haavard-avatar.jpg';
	import avatarLine from '$lib/assets/line-avatar.jpg';
	import avatarKa from '$lib/assets/ka-avatar.jpg';
</script>

<div class="container">
	<img class="quote-img quote1" src={quote} alt="icon av annførselstegn" />

	<div class="card">
		<p class="quote">
			“Raskt på pletten når han blir innkalt. Stabilt og godt resultat. Det merkes at Arve har stor
			interesse for faget. Han er dedikert, og bidrar til å holde vårt Steinway-flygel i toppform”
		</p>
		<div class="profile">
			<img class="avatar" src={avatarHaavard} alt="" />
			<div class="profile__info">
				<p class="name">Håvard Amlie</p>
				<p class="who">Kirketjener i Ås kirke - Vestre Toten</p>
			</div>
		</div>
	</div>
	<div class="card">
		<p class="quote">
			“Musikklinja ved Gjøvik Vgs setter stor pris på en fast kontrakt og det gode samarbeidet med
			Innlandet Piano om stemming og vedlikehold av skolens pianoer og flygler”
		</p>
		<div class="profile">
			<img class="avatar" src={avatarLine} alt="" />
			<div class="profile__info">
				<p class="name">Line Løvland Øftsaas</p>
				<p class="who">Pianist og avdelingsleder for musikklinja - Gjøvik Vgs</p>
			</div>
		</div>
	</div>
	<div class="card">
		<p class="quote">
			"Jeg er hele tiden nødt til å holde instrumentene mine klare for både konserter og alskens
			kreative innfall. Arve er kjempedyktig, og det er alltid en glede å spille etter at han har
			vært innom"
		</p>
		<div class="profile">
			<img class="avatar" src={avatarKa} alt="" />
			<div class="profile__info">
				<p class="name">Knut Anders Sørum</p>
				<p class="who">Komponist, musiker og sanger</p>
			</div>
		</div>
	</div>
	<img class="quote-img quote2" src={quote} alt="icon av annførselstegn" />
</div>

<style>
	p {
		color: var(--dark);
	}
	.container {
		max-width: 375px;
		margin: 0 auto;
		position: relative;
	}

	.card {
		margin: 48px 0;
	}

	.profile {
		display: flex;
		align-items: center;
		gap: 24px;
		margin-top: 16px;
	}

	.quote {
		font-size: 20px;
	}

	.name {
		font-size: 20px;
		font-weight: 600;
	}

	.avatar {
		width: 72px;
		height: 72px;
	}
	.quote-img {
		position: absolute;
	}

	.quote1 {
		top: 0;
		left: 0;
	}

	.quote2 {
		bottom: 0;
		right: 0;
	}
</style>
