<!-- ? Start Script -->
<script>
	export let name;
	import Header from './components/Header.svelte'

	const items = [
		{title: 'site1'},
		{title: 'site2'},
		{title: 'site3'},
	]
</script>

<!-- ? End Script -------------------------------------------------------------------->
<!-- * =============================================================================-->
<!-- # Start HTML -->

<div class="main">
	<h1>Hello {name}!</h1>
	<Header items={items} />
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
</div>
<!-- # End HTML ---------------------------------------------------------------------->
<!-- * =============================================================================-->
<!-- ^ Start CSS -->

<style>
	.main {
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
		.main {
			max-width: none;
		}
	}
</style>
<!-- ^ End CSS --------------------------------------------------------------->
