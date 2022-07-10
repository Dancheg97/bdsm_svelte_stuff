<script>
	let userImage =
		'https://thumbs.dreamstime.com/b/man-hipster-avatar-cartoon-guy-black-hair-man-hipster-avatar-cartoon-guy-black-hair-flat-icon-blue-background-user-223717055.jpg';
	let unfoldImage =
		'https://icon-library.com/images/hamburger-menu-icon-png-white/hamburger-menu-icon-png-white-14.jpg';
	let settingsImage =
		'https://icon-library.com/images/white-settings-icon/white-settings-icon-1.jpg';
	let exitImage = 'https://icon-library.com/images/logout-icon-png/logout-icon-png-13.jpg';
	export let onClick;
	$: innerWidth = 0;
	$: fillWidth = innerWidth - 130;
	$: innerHeight = 0;
	$: fillHeight = innerHeight - 209;
</script>

<svelte:window bind:innerWidth bind:innerHeight />

<body>
	<div class="flex-container">
		<img src={userImage} alt="" />
		<div class="spacer" style="--fill-width: {fillWidth}px" />
		<img src={unfoldImage} alt="" on:click={onClick} />
	</div>

	<div class="flex-container">
		<img src={settingsImage} alt="" />
	</div>

	<div class="flex-container">
		<img src={exitImage} alt="" />
	</div>

	<div class="vertical-spacer" style="--fill-height: {fillHeight}" />
</body>

<style>
	body {
		background-color: #001c41;
	}
	.flex-container {
		display: flex;
		flex-direction: row;
		padding: 5px;
		border-radius: 17px;
		height: min-content;
	}
	.spacer {
		width: var(--fill-width);
	}
	.vertical-spacer {
		height: var(--fill-height);
	}
	img {
		height: 45px;
		width: 45px;
		border-radius: 17px;
		padding: 4px;
	}
	div {
		display: flex;
		flex-direction: column;
		padding: 5px;
	}
</style>
