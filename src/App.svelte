<script lang="ts">
const name = 'Svelte'
const tag = `<h1>Svelte Kit</h1>`
const id = 'svelte-kit'
const disabled = false
const games = ['god of war', 'spiderman', 'last of us']
const num = 10;
</script>

<main>

<h1>Hello {name} from {@html tag}</h1>

    {#if ((num & 1)===0)}
    <p>Even</p>
    {:else}
    <p>Odd</p>
    {/if}

    {#each games as game}
    <p>{game}</p>
    {/each}


</main>

<style>

</style>
