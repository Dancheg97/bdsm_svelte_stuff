<script>
	import Content from './Content/Content.svelte';
	import accordion from './TopBar/accordion.js';
</script>

<details use:accordion>
	<summary>
		<span>I'm an accordion, click me!</span>
	</summary>
	<div class="flex-container">
		<Content />
	</div>
</details>

<style>
	.flex-container {
		display: flex;
		flex-direction: column;
	}
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
</style>
