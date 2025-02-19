<script>
	import Baltimore from "./Baltimore.svelte";
	import SanDiego from "./SanDiego.svelte";
	import { getTypography } from "$lib/components/foundations/typography/index";

	let activeTab = "San Diego"; // Default tab
</script>



<button class={getTypography('body','body','min-w-[4.563rem] max-h-[5rem] mx-auto flex items-center justify-center text-center outline-offset-4 outline-2 border active:outline focus:outline disabled:cursor-not-allowed disabled:outline-0 px-4 py-[0.625rem] rounded-[2.5rem] gap-1 text-d1 *:max-h-5 bg-primary text-common-white outline-primary border-primary hover:bg-primary-ultradark active:bg-primary focus:bg-primary-ultradark disabled:text-grey-500 disabled:bg-grey-100 col-start-2 col-end-2 row-start-3 row-end-3 my-4')}>Reserva ya</button>

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