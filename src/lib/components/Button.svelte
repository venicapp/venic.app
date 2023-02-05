<script>
	export let type = '';
	export let href = '';
</script>

{#if href}
	<a class="button-{type}" {href}>
		<slot />
	</a>
{:else}
	<button class="button-{type}" on:click>
		<slot />
	</button>
{/if}

<style>
    [class*="button-"] {
        @apply rounded-lg flex items-center py-3 px-6;
    }

	.button-primary {
		@apply shadow-xl shadow-white/10 font-semibold text-black bg-white;
	}
	.button-secondary {
		@apply font-semibold text-purple-100 bg-purple-400/10 ring-1 ring-purple-400/20 ring-inset rounded-lg;
	}
</style>
