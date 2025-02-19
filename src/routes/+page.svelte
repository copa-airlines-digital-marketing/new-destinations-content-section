<script>
	import Baltimore from "./Baltimore.svelte";
	import SanDiego from "./SanDiego.svelte";

	let activeTab = "San Diego"; // Default tab
</script>




<nav class="button container mx-auto p-4 gap-2">
	<button class="bg-primary " on:click={() => activeTab = "Baltimore"} class:active={activeTab === "Baltimore"}>Baltimore</button>
	<button class="bg-primary" on:click={() => activeTab = "SanDiego"} class:active={activeTab === "SanDiego"}>San Diego</button>
</nav>
<div class="content">
	{#if activeTab === "Baltimore"}
		<Baltimore />
	{:else if activeTab === "SanDiego"}
		<SanDiego />
	{/if}
</div>

<style>

	button {
		padding: 10px 20px;
		border: none;
		background: #ddd;
		cursor: pointer;
	}


</style>