<script>
	import Nav from "../components/Nav.svelte";
</script>

<main>
	<slot></slot>
	<Nav></Nav>
</main>

<style>
	:root {
		--nav-size: 3rem;
		font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
	}

	:global(*) {
		box-sizing: border-box;
	}

	:global(body) {
		margin: 0;
	}

	main {
		display: flex;
		flex-flow: column;
		justify-content: space-between;
		min-height: 100vh;
		padding: 1em;
		padding-bottom: var(--nav-size);
		position: relative;
	}
</style>