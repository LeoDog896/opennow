<script lang="ts">
	import Tailwindcss from "./Tailwindcss.svelte"

	let url: string

</script>

<Tailwindcss />
<input bind:value={url} placeholder="Type in a URL">
<button on:click={() => location.href = url}>Go</button>
