<script>
  import { onMount } from "svelte";
    import { planData } from "../store";
    export let itemList;

    onMount(() => {
        console.log(itemList);
    })
</script>

<main class="list">
    <ul>
        {#each 
            itemList as item}
            <li>{item}</li>
        {/each}
    </ul>
</main>

<style>

    /* main {
        border: 1px solid #000;
        border-radius: 10px;
        padding: 10px;
    } */
</style>

