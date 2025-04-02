<script>
	import Baltimore from "./Baltimore-ES.svelte/+page.svelte";
	import SanDiego from "./SanDiego-ES.svelte/+page.svelte";
	import Salta from "./Salta-ES.svelte/+page.svelte";
	import Tucuman from "./Tucuman-ES.svelte/+page.svelte";

	let activeTab = "San Diego"; // Default tab
</script>


<div class="container mx-auto my-8">
    <nav >
        <ol class="flex flex-col gap-3">
			<li><a href="./Salta-ES.svelte">Salta - ES</a></li>
            <li><a href="./Tucuman-ES.svelte">San Diego - ES</a></li>
            <li><a href="./Baltimore-ES.svelte">Baltimore</a></li>
            <li><a href="./SanDiego-ES.svelte">San Diego - ES</a></li>
            <li><a href="./SanDiego-EN.svelte">San Diego - EN</a></li>
            <li><a href="./SanDiego-PT.svelte">San Diego - PT</a></li>
            <li><a href="./SanDiego-FR.svelte">San Diego - FR</a></li>
        </ol>
	</nav>
</div>


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