<script>
	import Button from '$lib/components/Button.svelte';
	import NavHost from '../../layout/Navbar/NavHost.svelte';
</script>

<NavHost />
<main class="wrapper my-8">
	<div class="w-3/5 mx-auto">
		<h1 class="font-medium text-xl pb-2">Create your account</h1>
		<form class="flex flex-col gap-8 mt-4">
			<div class="flex flex-col gap-2">
				<label for="email" class="text-sm text-zinc-300">Email</label>
				<input
					type="email"
					class="rounded-md px-3 py-2 text-sm bg-transparent border border-zinc-700"
					id="email"
					name="email"
				/>
			</div>
			<div class="flex flex-col gap-2">
				<label for="display-name" class="text-sm text-zinc-300">Display name</label>
				<input
					type="text"
					class="rounded-md px-3 py-2 text-sm bg-transparent border border-zinc-700"
					id="display-name"
					name="display-name"
				/>
			</div>
			<div class="flex flex-col gap-2">
				<label for="username" class="text-sm text-zinc-300">Username</label>
				<input
					type="text"
					class="rounded-md px-3 py-2 text-sm bg-transparent border border-zinc-700"
					id="username"
					name="username"
				/>
			</div>
			<div class="flex flex-col gap-2">
				<label for="password" class="text-sm text-zinc-300">Password</label>
				<input
					type="text"
					class="rounded-md px-3 py-2 text-sm bg-transparent border border-zinc-700"
					id="password"
					name="password"
				/>
			</div>
			<Button type="primary">Create account</Button>
			<p class="text-sm text-zinc-500">
				By creating an account, you accept to our
				<a href="/tos" class="text-white font-medium"> Terms of Service </a>
				and <a href="/login" class="text-white font-medium">Privacy Policy</a>. Already have an
				account? <a href="/login" class="text-white font-medium">Log in.</a>
			</p>
		</form>
	</div>
</main>
