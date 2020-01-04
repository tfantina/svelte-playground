<script>
	export let name;
	import Playgrounds from './Playgrounds.svelte'
	import {counter} from "./stores.js";
</script>
{$counter}
<main>
	<h1>Svelte Playground</h1>
	<Playgrounds />
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
