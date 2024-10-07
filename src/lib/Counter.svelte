<script lang="ts">
  let count: number = 0
  function increment() {
    count++
  }
</script>

<main>
  <h2>Counter</h2>
  <p>Count: {count}</p>
  <button on:click={increment}>Increment</button>
</main>
