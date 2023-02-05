<script>
	import '../app.css';
</script>

<slot/>

<svelte:head>
	<link rel="stylesheet" href="https://rsms.me/inter/inter.css">
	<meta charset="UTF-8" />
	<meta name="viewport" content="width=device-width, initial-scale=1.0" />
	<meta name="og:title" content="Venic" />
	<meta content="/venic_logo.webp" property="og:image" />
	<meta property="og:description" content="An open-sourced, community-driven service designed to help creators sell their content to the world." />
	<meta name="twitter:image" itemprop="image" content="/venic_logo.webp" />
	<meta name="twitter:card" content="summary" />
	<meta name="theme-color" content="#B12B8D" />
	<title>Venic</title>
</svelte:head>
