<script>
	import Note from '$lib/assets/note-vektor.svelte';
</script>

<div class="wrapper">
	<div class="container">
		<div class="text">
			<h2>Presentasjonsvideo</h2>
			<p>
				Stemming av flygler og pianoer er et eget yrke som det krever år med trening for å beherske
				– et spennende kompromiss av musikalske preferanser og fysiske lover.
			</p>
			<p class="last-p">
				Arve Øfstaas er utdannet Pianostemmer og pianotekniker fra Norges Musikkhøgskole. Han ble
				uteksaminert i 2019 og er en av de fem første studentene i Norge som fikk ta denne
				musikkfaglig utdanningen på høgskolenivå
			</p>
		</div>
		<div class="video-container">
			<div class="video" style="position:relative;">
				<iframe
					src="https://player.vimeo.com/video/805630829?h=5b8408e6d1&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479"
					frameborder="0"
					allow="autoplay; fullscreen; picture-in-picture"
					allowfullscreen
					style="position:absolute;top:0;left:0;width:100%;height:100%;"
					title="Main Edit Innlandet Piano 16x9 COMPRESSED.mov"
				/>
			</div>
		</div>
		<div class="note-container">
			<Note />
		</div>
	</div>
</div>

<style>
	.wrapper {
		background: var(--primary);
		display: flex;
		justify-content: center;
		overflow: hidden;
	}

	.container {
		position: relative;
		z-index: 0;
		max-width: 1440px;
	}

	.text {
		max-width: 1024px;
		margin: 48px auto 0;
		color: #fff5f6;
		position: relative;
		z-index: 1;
		padding-inline: 5%;
	}

	h2 {
		font-size: 25px;
	}

	p {
		font-size: 16px;
		margin-top: 24px;
	}

	.last-p {
		margin-top: 16px;
	}

	.video-container {
		padding-inline: 5%;
	}

	.video {
		margin: 24px auto 64px auto;
		aspect-ratio: 16/9;
		max-width: 1024px;
		z-index: 1;
	}

	.note-container {
		position: absolute;
		width: 100%;
		transform: rotate(-32deg);
		scale: 1.35;
		top: 15%;
		pointer-events: none;
	}

	@media screen and (min-width: 768px) {
		.note-container {
			scale: 1.4;
			top: 24%;
		}
	}

	@media screen and (min-width: 960px) {
		.text {
			text-align: center;
			padding-inline: 10%;
		}
	}
</style>
