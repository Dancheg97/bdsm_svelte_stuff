<script>
	import Button from './Button.svelte';

	let userImg =
		'https://thumbs.dreamstime.com/b/man-hipster-avatar-cartoon-guy-black-hair-man-hipster-avatar-cartoon-guy-black-hair-flat-icon-blue-background-user-223717055.jpg';
	let homeImage = 'https://icon-library.com/images/white-home-icon-png/white-home-icon-png-21.jpg';

	let settingsImage =
		'https://icon-library.com/images/white-settings-icon/white-settings-icon-1.jpg';
	let exitImage = 'https://icon-library.com/images/logout-icon-png/logout-icon-png-13.jpg';
</script>

<div>
	<ul>
		<li>
			<Button src={userImg} />
		</li>
		<hr />
		<li>
			<Button src={homeImage} />
		</li>
		<li>
			<Button src={settingsImage} />
		</li>
		<div class="spacer" />
		<hr />
		<li>
			<Button src={exitImage} />
		</li>
	</ul>
</div>

<style>
	div {
		background-color: #001c41;
		width: min-content;
		border-radius: 17px;
	}
	ul {
		list-style-type: none;
		margin: 0;
		width: min-content;

		padding-top: 10px;
		padding-right: 10px;
		padding-bottom: 10px;
		padding-left: 10px;
	}
	div.spacer {
		height: 100%;
	}
</style>
