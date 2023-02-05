<script>
	import NavButton from './NavButton.svelte';
</script>

<nav class="px-10 py-6 flex items-center justify-between">
	<a href="/" class=" flex items-center gap-4">
		<img
			class="w-6 h-6"
			alt="logo"
			src="/venic_logo.webp"
		/>
		<div class="text-xl font-semibold">Venic</div>
	</a>
	<div class="flex gap-8">
		<NavButton href="/blog">Blog</NavButton>
		<NavButton href="https://github.com/venicme">Github</NavButton>
		<NavButton href="https://discord.gg/dC8FHPXuQG">Discord</NavButton>
	</div>
</nav>
