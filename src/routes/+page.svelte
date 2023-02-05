<script>
	import Button from "$lib/components/Button.svelte";
	import NavHost from "../layout/Navbar/NavHost.svelte";
</script>

<NavHost/>
<main class="wrapper my-8">
	<div class="blur-wrapper">
		<div class="blur-left"></div>
		<div class="blur-right"></div>
	</div>
	<section class="flex items-center text-center justify-center flex-col">
		<div class="text-xs text-purple-300 bg-purple-300/10 py-1.5 px-3 mb-2 rounded-full ring-1 ring-purple-400/20 ring-inset backdrop-blur-lg">
			Alpha Stage
		</div>
		<h1 class="font-medium text-7xl text-transparent bg-clip-text bg-gradient-to-br from-white to-zinc-400 pb-2">
			Venic is the future of commissioning
		</h1>
		<p class="text-gray-400 text-xl w-2/4 mt-4">
			An open-sourced, community-driven platform designed to help creators sell their content to the world. 
		</p>
	</section>
	<div class="mt-8 flex items-center text-center justify-center gap-4">
		<Button type="primary">
			Sign up →
		</Button>
		<Button type="secondary" href="https://discord.gg/dC8FHPXuQG">Join the Discord</Button>
	</div>

    <img class="mt-16 w-4/5 mx-auto rounded-xl shadow-2xl shadow-blue-500/20" src="/hero.webp" alt="profile page"/>
	
	<div class="h-100 w-100 bg-black bg-[radial-gradient(#123_0.5px,#000_2.4px)] bg-[37px_37px]"/>
</main>

<hr/>

<main class="wrapper my-16">
	<section class="">
		<div class="max-w-max text-xs text-purple-300 bg-purple-300/10 py-1.5 px-3 mb-2 rounded-full ring-1 ring-purple-400/20 ring-inset">
			Revenue
		</div>
		<h2 class="font-medium text-4xl text-transparent bg-clip-text bg-gradient-to-br from-white to-zinc-400 pb-2">
			Your work, your money.
		</h2>
		<p class="text-gray-400 text-md mt-1 w-2/3">
			Venic always keeps the best interest of creators in mind. Get paid 100% of the revenue — we never take a cut (unless you want us to).
		</p>
	</section>
</main>

<hr/>

<main class="wrapper my-16">
	<section class="">
		<div class="max-w-max text-xs text-purple-300 bg-purple-300/10 py-1.5 px-3 mb-2 rounded-full ring-1 ring-purple-400/20 ring-inset">
			Talent
		</div>
		<h2 class="font-medium text-4xl text-transparent bg-clip-text bg-gradient-to-br from-white to-zinc-400 pb-2">Find just about anything.</h2>
		<p class="text-gray-400 text-md mt-1 w-2/3">
			Many things many people many service ceiuceiurgfieurfydu98 help how to write
		</p>
	</section>
</main>

<div class="dots"/>

<style>
	.dots {
		position: absolute;
		top: 0;
		left: 0;
		width: 100vw;
		height: 100%;
		z-index: -999;
		background: linear-gradient(180deg, transparent 0, theme("colors.black") 300px),
        	fixed 0 0 /20px 20px radial-gradient(theme("colors.zinc.700") 1px, transparent 0),
        	fixed 10px 10px /20px 20px radial-gradient(theme("colors.zinc.700") 1px, transparent 0);
	}

	.blur-wrapper {
		filter: blur(175px);
		z-index: -4;
		top: -360px;
		right: 0;
		bottom: 0;
		left: 0;
		max-width: 750px;
		margin: 0 auto;
		position: absolute;
	}

	.blur-left {
		position: absolute;
		width: 400px;
		height: 400px;
		z-index: -99;
		top: 5%;
		left: -15%;
		background: #ba2b8565;
	}
	
	.blur-right {
		background: #493be894;
		position: absolute;
		width: 400px;
		height: 400px;
		z-index: -99;
		top: 5%;
		right: -15%;
	}
</style>