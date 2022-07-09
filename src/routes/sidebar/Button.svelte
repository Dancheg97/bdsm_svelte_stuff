<script>
	export let src = 'https://icon-library.com/images/logout-icon-png/logout-icon-png-13.jpg';
	export function onClick() {
		alert('clicked');
	}
</script>

<img {src} alt="" on:click={onClick} />

<style>
	img {
		height: 45px;
		width: 45px;
		border-radius: 17px;
		padding: 4px;
	}
</style>
