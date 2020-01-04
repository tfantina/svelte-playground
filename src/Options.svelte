<script>
export let buttons;
export let selectOption;

</script>

{#each buttons as btn}
<button on:click={selectOption(btn)}>{btn}</button>
{/each}
