<script lang="ts">
	import Tailwindcss from "./Tailwindcss.svelte"

	let url: string

</script>

<Tailwindcss />
<div class="flex justify-center items-center h-screen">
	<div class="border-2 border-solid p-16 border-slate-400">
		<input class="m-4 p-2 border-solid border-2 border-" bind:value={url} placeholder="Type in a URL">
		<button class="px-10 px-5 border-solid border-2 border-lime-400" on:click={() => location.href = url}>Go</button>
	</div>
</div>