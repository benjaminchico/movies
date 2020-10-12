<script>
	import Card from './Card/Card.svelte'
	export let name;
	let texto = "Este es el bebe"
</script>

<svelte:head>
	<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" integrity="sha384-JcKb8q3iqJ61gNV9KGb8thSsNjpSL0n8PARn9HuZOnIxN0hoP+VmmDGMN5t9UJ0Z" crossorigin="anonymous">
</svelte:head>
<title>Movies svelte</title>
<main>
	<h1>Hello {name}!</h1>
	 <h5>{texto}</h5>
	<input type="text" bind:value={texto}>
	<Card title="COBAYAS"></Card>
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