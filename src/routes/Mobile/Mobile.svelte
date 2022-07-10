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
	<TopList onClick={fold} />
{/if}
