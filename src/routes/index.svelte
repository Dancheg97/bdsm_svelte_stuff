<script>
	import Desktop from './Desktop/Desktop.svelte';
	import Mobile from './Mobile/Mobile.svelte';

	$: innerWidth = 0;
</script>

<svelte:window bind:innerWidth />

{#if innerWidth > 500}
	<Desktop />
{:else}
	<Mobile />
{/if}

<style>
	:global(body) {
		background-color: #1d3040;
		color: #bfc2c7;
	}
</style>
