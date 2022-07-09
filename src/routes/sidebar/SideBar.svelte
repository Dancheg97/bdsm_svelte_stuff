<script>
	import Button from './Button.svelte';

	$: innerHeight = 0;
	$: sideBarHeight = innerHeight - 16;
	$: omitHeight = sideBarHeight - 268;

	let userImg =
		'https://thumbs.dreamstime.com/b/man-hipster-avatar-cartoon-guy-black-hair-man-hipster-avatar-cartoon-guy-black-hair-flat-icon-blue-background-user-223717055.jpg';
	let homeImage = 'https://icon-library.com/images/white-home-icon-png/white-home-icon-png-21.jpg';

	let settingsImage =
		'https://icon-library.com/images/white-settings-icon/white-settings-icon-1.jpg';
	let exitImage = 'https://icon-library.com/images/logout-icon-png/logout-icon-png-13.jpg';
</script>

<svelte:window bind:innerHeight />

<div class="flex-container" style="--screen-height: {sideBarHeight}px">
	<Button src={userImg} />
	<Button src={homeImage} />
	<Button src={settingsImage} />
	<div class="spacer" style="--omit-height: {omitHeight}px" />
	<Button src={exitImage} />
</div>

<style>
	div {
		background-color: #001c41;
		width: min-content;
		border-radius: 17px;
		height: var(--screen-height);
	}
	.spacer {
		height: var(--omit-height);
	}
</style>
