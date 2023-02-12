<script>
	import Button from '$lib/components/Button.svelte';
	import Chip from '$lib/components/Chip.svelte';
	import { numberFormat } from '$lib/util';

	let username = 'afn';
	let bio = 'the only Venic profile (literally)';
	let user_tags = ['Digital Artist', 'Web Developer', 'UI/UX Designer'];
	
    let followers = 109;
	let following = 1;
	let views = 121029;

	let completed_commissions = 3;
	let rating = 4.8;
</script>

<header class="flex justify-between items-center pb-8">
	<div class="flex gap-8 items-center">
		<div
			style="background-image:url('https://github.com/xafn.png');"
			class="h-40 w-40 rounded-full bg-cover bg-zinc-900"
		/>
		<div class="pt-2">
			<h1 class="font-semibold text-4xl pb-1">{username}</h1>
			{#if bio}
				<p class="text-sm mt-2">{bio}</p>
			{/if}
			{#if user_tags}
				<div class="flex gap-2">
					{#each user_tags as tag}
						<a
							href="/tags/{tag.replace(/\W+(?!$)/g, '-').toLowerCase()}"
							class="text-sm mt-2 text-zinc-400">{tag}</a
						>
					{/each}
				</div>
			{/if}
		</div>
	</div>
	<div class="flex gap-2 h-max">
		<Button rounded type="secondary">Follow</Button>
		<Button rounded type="primary">Commission</Button>
	</div>
</header>

<section class="p-6 bg-zinc-900 rounded-xl w-[32rem] mb-4">
	<h2 class="text-sm text-zinc-400 uppercase pb-2">Info</h2>
	<div class="flex flex-wrap gap-2">
        <Chip>{numberFormat.format(followers)} followers</Chip>
        <Chip>{numberFormat.format(following)} following</Chip>
        <Chip>{numberFormat.format(views)} views</Chip>

		{#if completed_commissions}
			<Chip>{numberFormat.format(completed_commissions)} commissions</Chip>
		{/if}
		{#if rating}
			<Chip>{rating}/5 rating</Chip>
		{/if}
        <!-- ill fix later -->
		<Chip>~4h response time</Chip>
		<Chip>~1w delivery time</Chip>
	</div>
</section>
<section class="p-6 bg-zinc-900 rounded-xl w-[32rem]">
	<h2 class="text-sm text-zinc-400 uppercase pb-2">Reviews (2)</h2>
	<div class="flex flex-wrap gap-2" />
</section>
