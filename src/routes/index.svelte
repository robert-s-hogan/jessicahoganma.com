<script context="module">
	export const prerender = true;
</script>

<script>
	import Header from '$lib/header/Header.svelte';
	import Services from '$lib/services/Services.svelte';
	import Quote from '$lib/quote/Quote.svelte';
	import AboutMe from '$lib/aboutMe/AboutMe.svelte';
	import GetInTouch from '$lib/getInTouch/GetInTouch.svelte';
	import Contact from '$lib/contact/Contact.svelte';
	import Portfolio from '$lib/portfolio/Portfolio.svelte';

	import Modal from "$lib/modal/Modal.svelte";

	let open = false;

	let showPopup = false;
	const onShowPopup = (ev) => {
		showPopup = true;
	}
	const onPopupClose = (data) => {
		showPopup = false;
		console.log(data);
	};
</script>

<svelte:head>
	<title>Data Scientist and Data Analyst - Jessica Hogan M.A.	</title>
	<meta name="description" content="I want to help you make the best data-driven decisions and translate data into actionable insights. I have experience with SQL, Excel, reporting, dashboards and statistics - Jessica Hogan M.A.">
</svelte:head>

<section class="bg-gradient-to-br from-peach to-mint" style="max-width: 100%; height: 80vh;">
	<!-- <Sidebar bind:open/>
	<Navbar bind:sidebar={open}/> -->
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
		<p class="text-gray-700 text-lg py-2 w-4/5">I want to help you make the best data-driven decisions and translate data into actionable insights.
		</p>
		<div class="my-4 flex flex-col justify-center md:flex-row md:space-between">

			<button class="bg-orange hover:opacity-80 px-8 py-2 rounded-lg text-lg text-white" on:click={onShowPopup}>Contact me</button>
			<a href="#portfolio" class="px-8 py-2 rounded-lg hover:no-underline pt-4 md:pt-4">
				<p class="align-middle text-green hover:text-slate text-lg">See My Work 					
					<svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 inline pb-1" fill="none" viewBox="0 0 24 24" stroke="currentColor">
						<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14 5l7 7m0 0l-7 7m7-7H3" />
					</svg>
				</p>
			</a>
		</div>
	</div>
</section>

<!-- <Quote /> -->

<Portfolio />

<!-- <Services /> -->

<AboutMe />

<section class="max-w-6xl mx-auto pb-8 text-white text-center -mt-16">
	<div class="w-11/12 lg:w-full mx-auto bg-orange text-white rounded-lg shadow-lg overflow-hidden">
		<div class="flex flex-col md:flex-row md:items-center md:space-x-6 w-11/12 lg:w-3/4 mx-auto justify-center py-8">
				<h2 class="text-white text-2xl font-semibold">
					Start a project
				</h2>
				<p class="mt-2 text-white md:flex-auto">
					Interested in working together? <span class="md:block"></span>We should queue up a
					chat. I’ll buy the coffee.
				</p>
				<button on:click={onShowPopup} class="rounded-lg mx-auto mt-6 md:mt-0 md:py-3 md:px-4 md:rounded-full py-3 px-10 hover:text-orange hover:bg-white font-semibold border-2 md:w-1/4 bg-orange text-white">
					Let's do this
				</button>
		</div>
	</div>
</section>


<!-- <Contact /> -->



<Modal open={showPopup} onClosed={(data) => onPopupClose(data)} />



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
	