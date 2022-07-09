<script>
	export let userImage =
		'https://thumbs.dreamstime.com/b/man-hipster-avatar-cartoon-guy-black-hair-man-hipster-avatar-cartoon-guy-black-hair-flat-icon-blue-background-user-223717055.jpg';
	export let unfoldImage =
		'https://icon-library.com/images/hamburger-menu-icon-png-white/hamburger-menu-icon-png-white-14.jpg';
	export function onClick() {
		alert('clicked');
	}
	$: innerWidth = 0;
	$: fillWidth = innerWidth - 120;
</script>

<svelte:window bind:innerWidth />

<div class="flex-container">
	<img src={userImage} alt="" />
	<div class="spacer" style="--fill-width: {fillWidth}px" />
	<img src={unfoldImage} alt="" />
</div>

<style>
	img {
		height: 45px;
		width: 45px;
		border-radius: 17px;
		padding: 4px;
	}
	div {
		padding: 5px;
	}
	.flex-container {
		display: flex;
		flex-direction: row;
	}
	.spacer {
		width: var(--fill-width);
	}
</style>
