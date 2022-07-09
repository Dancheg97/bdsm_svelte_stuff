<script>
	import SideBar from './SideBar/SideBar.svelte';
	import Content from './Content/Content.svelte';
</script>

<div class="flex-container">
	<SideBar />
	<Content />
</div>

<style>
	:global(body) {
		background-color: #1d3040;
		color: #bfc2c7;
	}
	.flex-container {
		display: flex;
		flex-direction: row;
	}
</style>
