<script>
	import Content from '../Content/Content.svelte';
	import SideBar from '../SideBar/SideBar.svelte';
</script>

<div class="flex-container">
	<SideBar />
	<Content />
</div>

<style>
	.flex-container {
		display: flex;
		flex-direction: row;
	}
</style>
