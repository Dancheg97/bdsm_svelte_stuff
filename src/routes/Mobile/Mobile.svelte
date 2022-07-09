<script>
	import Content from './Content/Content.svelte';
	import accordion from './accordion.js';
	import TopMenu from './TopBar/TopMenu.svelte';
	import TopList from './TopBar/TopList.svelte';
</script>

<details use:accordion>
	<summary>
		<TopMenu />
	</summary>
	<TopList />
</details>
<Content />

<style>
	details {
		background: #001c41;
		height: var(--collapsed);
		overflow: hidden;
		transition: height 300ms cubic-bezier(0.4, 0.01, 0.165, 0.99);
		border-radius: 5px;
	}
	details[open] {
		height: var(--expanded);
	}
	summary {
		display: block;
		padding-bottom: 0.5rem;
		padding-top: 0.5rem;
		padding-inline-end: 0.5rem;
		padding-inline-start: 1rem;
	}
</style>
