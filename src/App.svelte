<script lang="ts">
 import ShipContainer from "./ShipContainer.svelte";

 export let name: string;
</script>

<main>
	<h1>{name}</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
    <hline/>
    <div id="containerlists">
        <ShipContainer/>
    </div>
</main>

<style>
	#containerlists {
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
