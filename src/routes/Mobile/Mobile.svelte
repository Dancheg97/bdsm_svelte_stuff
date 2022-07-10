<script>
	import Content from './Content/Content.svelte';
	import TopMenu from './TopBar/TopMenu.svelte';
	import TopList from './TopBar/TopList.svelte';
	$: innerWidth = 0;
	$: actualWidth = innerWidth - 20;
</script>

<svelte:window bind:innerWidth />

<div class="flex-container" style="--screen-height: {actualWidth}px">
	<TopMenu />
</div>

<TopList />
<Content />

<style>
	div {
		background-color: #001c41;
		width: var(--screen-height);
		border-radius: 17px;
		height: min-content;
	}
</style>
