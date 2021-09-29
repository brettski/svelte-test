<script>
	export let name;
	const mssg = __testApp.env.BRETT_S;
	const nodeenv = __testApp.env.NODE_ENV;
	const nodever = __testApp.env.NODE_VER;
	
</script>

<main>
	<h1>Hello {name}!</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
	<p>This is our env message: <strong>{mssg}</strong></p>
	<p>NODE_ENV: {nodeenv}</p>
	<p>node version: {nodever}</p>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>
