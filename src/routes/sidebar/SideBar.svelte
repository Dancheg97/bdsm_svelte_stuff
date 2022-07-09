<script>
	import Button from './Button.svelte';

	const srcs = [
		'https://thumbs.dreamstime.com/b/man-hipster-avatar-cartoon-guy-black-hair-man-hipster-avatar-cartoon-guy-black-hair-flat-icon-blue-background-user-223717055.jpg',
		'https://icon-library.com/images/white-home-icon-png/white-home-icon-png-21.jpg',
		'https://icon-library.com/images/white-settings-icon/white-settings-icon-1.jpg',
		'https://icon-library.com/images/logout-icon-png/logout-icon-png-13.jpg'
	];
</script>

<ul>
	{#each srcs as src}
		<li>
			<Button src />
		</li>
	{/each}
</ul>
