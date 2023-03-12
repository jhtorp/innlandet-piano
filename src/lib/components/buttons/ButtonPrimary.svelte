<button> <slot /> </button>

<style>
	button {
		border: none;
		background: var(--light);
		border: 2px solid transparent;
		color: var(--dark);
		cursor: pointer;
		transition: 0.2s;
		font-family: 'Barlow', sans-serif;
		width: 100%;
		height: 100%;
	}

	button:hover {
		background: none;
		border: 2px solid var(--light);
		color: var(--light);
	}
</style>
