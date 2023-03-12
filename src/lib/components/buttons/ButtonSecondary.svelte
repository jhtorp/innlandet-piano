<button> <slot /> </button>

<style>
	button {
		background: none;
		border: 2px solid var(--light);
		color: var(--light);
		cursor: pointer;
		transition: 0.2s;
		font-family: 'Barlow', sans-serif;
		width: 100%;
		height: 100%;
	}

	button:hover {
		background: var(--light);
		color: var(--dark);
	}
</style>
