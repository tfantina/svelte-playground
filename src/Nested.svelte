<script>
import NestedProp from './NestedProp.svelte'

let valueToPass = "";

</script>
<input bind:value={valueToPass} type="text" />

<NestedProp propertyPassed={valueToPass}/>
