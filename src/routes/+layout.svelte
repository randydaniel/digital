<script>
	import { dev } from '$app/environment';
	import { inject } from '@vercel/analytics';
	import '../app.css';

	inject({ mode: dev ? 'development' : 'production' });
</script>

<head>
	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" />
	<link
		href="https://fonts.googleapis.com/css2?family=IBM+Plex+Mono:wght@300&display=swap"
		rel="stylesheet"
	/>
</head>

<slot />

<style lang="postcss">
	:global(html) {
		background-color: theme(colors.black-200);
		color: white;
	}
</style>
