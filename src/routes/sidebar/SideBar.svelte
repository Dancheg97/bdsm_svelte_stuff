<script>
	import Button from './Button.svelte';

	let userImg =
		'https://thumbs.dreamstime.com/b/man-hipster-avatar-cartoon-guy-black-hair-man-hipster-avatar-cartoon-guy-black-hair-flat-icon-blue-background-user-223717055.jpg';
	let homeImage = 'https://icon-library.com/images/white-home-icon-png/white-home-icon-png-21.jpg';

	let settingsImage =
		'https://icon-library.com/images/white-settings-icon/white-settings-icon-1.jpg';
	let exitImage = 'https://icon-library.com/images/logout-icon-png/logout-icon-png-13.jpg';
</script>

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
	<hr />
	<li>
		<Button src={exitImage} />
	</li>
</ul>

<style>
	ul {
		list-style-type: none;
		margin: 0;
		padding: 0;
	}
</style>
