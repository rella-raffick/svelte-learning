<script lang="ts">

    let items = ['react', 'angular']

    $: amount = items.length

    function add() {
        items = [...items, items.length++]
    }
</script>
