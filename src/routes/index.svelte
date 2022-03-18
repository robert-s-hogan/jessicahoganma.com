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



<!-- <Quote /> -->

<Portfolio />

<!-- <Services /> -->

<AboutMe />

<section id="contact" class="max-w-6xl mx-auto pb-8 text-white text-center -mt-16">
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
