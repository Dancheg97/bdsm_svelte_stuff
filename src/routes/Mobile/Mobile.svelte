<script>
	import Content from './Content/Content.svelte';
	import TopMenu from './TopBar/TopMenu.svelte';
	import TopList from './TopBar/TopList.svelte';
	$: closed = true;

	function fold() {
		closed = !closed;
	}
</script>

{#if closed}
	<TopMenu onClick={fold} />
	<Content />
{:else}
	<div />
{/if}

<style>
	div {
		height: 100px;
		width: 100px;
		background-color: #001c41;
	}
</style>
