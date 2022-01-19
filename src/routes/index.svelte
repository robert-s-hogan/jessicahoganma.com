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
	// import Portfolio from '$lib/portfolio/Portfolio.svelte';
</script>

<svelte:head>
	<title>Home</title>
</svelte:head>


<Header />

<Quote />

<Services />

<AboutMe />

<GetInTouch />

<!-- <Portfolio /> -->

<Contact />
