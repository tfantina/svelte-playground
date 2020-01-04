<script>
import Reactivity from "./Reactivity.svelte"
import Nested from "./Nested.svelte"
import Store from "./Store.svelte"

import Options from "./Options.svelte"

let buttons = ["Reactivity", "Nested Properties", "Stores"];
let display;
let selectOption = (button) => {
  display = button;
  console.log(button)
}


</script>

<h3>Hello</h3>

<Options {selectOption} {buttons}/>

{#if display === "Reactivity"}
  <Reactivity />
{:else if display === "Nested Properties"}
  <Nested />
{:else if display === "Stores"}
  <Store />
{/if}
