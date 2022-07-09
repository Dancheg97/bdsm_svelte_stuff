<script>
	export let src = 'https://icon-library.com/images/logout-icon-png/logout-icon-png-13.jpg';
	function onClick() {
		alert('clicked');
	}
</script>

<!-- svelte-ignore a11y-img-redundant-alt -->
<img {src} alt="image is loading" />

<style>
	img {
		height: 45px;
		width: 45px;
		border-radius: 8px;
		padding: 4px;
	}
</style>
