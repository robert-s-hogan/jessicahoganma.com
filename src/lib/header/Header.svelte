<script>
	import Navbar from '$lib/navbar/Navbar.svelte';
	import Sidebar from '$lib/sidebar/Sidebar.svelte';
	import Hero from '$lib/img/hero_wavelength.svg';
    // import Profile from '$lib/img/linkedin_profile.jpeg';
	let open = false;
</script>

<section class="bg-gradient-to-br from-peach to-mint" style="max-width: 100%; height: 80vh;">
	<Sidebar bind:open/>
	<Navbar bind:sidebar={open}/>
	<div class="hero-text">
		<!-- <div class="mx-auto w-1/2 md:w-1/6 pb-4 ">
			<img src={Profile} alt="" class="rounded-lg" />
		</div> -->
		<h1 class="font-semibold text-4xl">
			Hi, I'm Jessica.<br />
			<span class="text-black bg-clip-text bg-gradient-to-br from-orange to-peach">
				Data Scientist and Data Analyst

			</span>
		</h1>
		<p class="text-gray-700 text-lg py-2 w-4/5">I want to help you make the best data-driven decisions
		</p>
		<div class="my-4 flex flex-col justify-center md:flex-row md:space-between">
			<button class="bg-orange hover:opacity-80 px-8 py-2 rounded-lg text-lg text-white">Contact me</button>
			<a href="#/portfolio" class="px-8 py-2 rounded-lg hover:no-underline pt-4 md:pt-4">
				<p class="align-middle text-green hover:text-slate text-lg">See My Work 					
					<svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 inline pb-1" fill="none" viewBox="0 0 24 24" stroke="currentColor">
						<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14 5l7 7m0 0l-7 7m7-7H3" />
					</svg>
				</p>
			</a>
		</div>
	</div>
</section>

<style>
	.hero-text {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 1;
		text-align: center;
		color: var(--tertiary-color);
		height: 100%;
	}
</style>