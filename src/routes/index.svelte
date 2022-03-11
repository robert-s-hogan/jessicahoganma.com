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
</script>

<svelte:head>
	<title>Data Scientist and Data Analyst - Jessica Hogan M.A.	</title>
	<meta name="description" content="I want to help you make the best data-driven decisions and translate data into actionable insights. I have experience with SQL, Excel, reporting, dashboards and statistics - Jessica Hogan M.A.">
</svelte:head>


<Header />

<!-- <Quote /> -->

<Portfolio />

<!-- <Services /> -->

<AboutMe />

<GetInTouch />


<!-- <Contact /> -->
