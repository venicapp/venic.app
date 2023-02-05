<script>
	import NavHost from "../layout/Navbar/NavHost.svelte";
</script>
<NavHost/>
<main class="wrapper my-8">
	<div class="blur-wrapper">
		<div class="blur-left"></div>
		<div class="blur-right"></div>
	</div>
	<section class="flex items-center text-center justify-center flex-col">
		<div
			class="text-xs text-purple-300 bg-purple-300/10 py-1.5 px-3 mb-2 rounded-full ring-1 ring-purple-400/20 ring-inset backdrop-blur-lg"
		>
			Alpha Release
		</div>
		<h1 class="font-medium text-7xl text-transparent bg-clip-text bg-gradient-to-br from-white to-zinc-400 pb-2">Venic is the future of commissioning</h1>
		<p class="text-gray-400 text-xl w-2/4 mt-4">
			An open-sourced, community-driven service designed to help creators sell their content to the world. 
		</p>
	</section>
	<div class="mt-8 flex items-center text-center justify-center gap-4">
		<button class="shadow-xl shadow-white/10 font-semibold text-black bg-white py-3 px-6 rounded-lg flex items-center">
			Sign up
			<svg
				class="stroke-2 fill-black w-4 h-4 ml-2"
				xmlns="http://www.w3.org/2000/svg"
				viewBox="0 0 48 48"
			>
				<path d="m18.75 36.7-2.85-2.85 9.9-9.9-9.9-9.9 2.85-2.85L31.5 23.95Z" />
			</svg>
		</button>
		<button class="font-semibold text-purple-100 bg-purple-400/10 ring-1 ring-purple-400/20 ring-inset py-3 px-6 rounded-lg"> Join the Discord </button>
	</div>

    <img class="mt-16 w-4/5 mx-auto rounded-xl shadow-2xl shadow-blue-500/20" src="https://cdn.discordapp.com/attachments/1071198785050521712/1071199004743979118/MacBook_Pro_14__-_2.png" alt="profile page"/>
	
	<div class="h-100 w-100 bg-black bg-[radial-gradient(#123_0.5px,#000_2.4px)] bg-[37px_37px]"/>
</main>

<hr/>

<main class="wrapper my-16">
	<section class="">
		<div
			class="max-w-max text-xs text-purple-300 bg-purple-300/10 py-1.5 px-3 mb-2 rounded-full ring-1 ring-purple-400/20 ring-inset"
		>
			Revenue
		</div>
		<h2 class="font-medium text-4xl text-transparent bg-clip-text bg-gradient-to-br from-white to-zinc-400 pb-2">Your work, your money.</h2>
		<p class="text-gray-400 text-md mt-1 w-2/3">
			Venic always keeps the best interest of creators in mind. Get paid 100% of the revenue; we will never take a cut (unless you want us to).
		</p>
	</section>
</main>
<hr/>

<main class="wrapper my-16">
	<section class="">
		<div
			class="max-w-max text-xs text-purple-300 bg-purple-300/10 py-1.5 px-3 mb-2 rounded-full ring-1 ring-purple-400/20 ring-inset"
		>
			Talent
		</div>
		<h2 class="font-medium text-4xl text-transparent bg-clip-text bg-gradient-to-br from-white to-zinc-400 pb-2">Find just about anything.</h2>
		<p class="text-gray-400 text-md mt-1 w-2/3">
			Many things many people many service ceiuceiurgfieurfydu98 help how to write
		</p>
	</section>
</main>


<style>
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