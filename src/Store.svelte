<script>
import {counter} from "./stores.js";
//
// let count;
//
// const unsubscribe = counter.subscribe(val => {
//   count = val;
// });

let updateCount = () => {
  counter.update(val => val + 1);
}
</script>

{$counter}
<button on:click={updateCount}>Update</button>
