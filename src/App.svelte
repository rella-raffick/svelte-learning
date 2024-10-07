<script lang="ts">
const name = 'Svelte'
const tag = `<h1>Svelte Kit</h1>`
const id = 'svelte-kit'
const disabled = false
let games = ['god of war', 'spiderman', 'last of us']
let songs_artist = [
    {song: 'Stairway to Heaven', artist: 'Led Zeppelin'},
    {song: 'Bohemian Rhapsody', artist: 'Queen'},
    {song: 'Yesterday', artist: 'The Beatles'}
]
const num = 10
let newGame = ''
function addNew(){
    games = [...games, newGame]
}
</script>

<main>

<h1>Hello {name} from {@html tag}</h1>

    {#if ((num & 1)===0)}
    <p>Even</p>
    {:else}
    <p>Odd</p>
    {/if}

    {#each games as game, i}
    <p>{i + 1 }. {game}</p>
    {/each}

    {#each songs_artist as {song, artist}}
    <p>{song} by {artist}</p>
    {/each}

    <input bind:value={newGame} type="text" />
    <button on:click={addNew}>Submit</button>


</main>

<style>

</style>
