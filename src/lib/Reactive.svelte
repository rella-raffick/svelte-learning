<script lang="ts">
let list = ['react', 'angular']

function add() {
  list = [...list, 'svelte']
}

</script>

<main>
  <h2>Reactive</h2>
  <ul>
    {#each list as item}
      <li>{item}</li>
    {/each}
  </ul>
    <button on:click={add}>Add Svelte</button>
</main>
