<script>
	import Header from '$lib/header/Header.svelte';
	import '../app.css';
</script>

<!-- <Header /> -->

<main>
	<slot />
</main>


<footer class="w-full mx-auto">
    <div class="px-6 py-12 bg-blue-100">
        <h2 class="uppercase border-b-2">LinkedIn</h2>
        <p class="py-4">We can get in touch via <a href="https://www.linkedin.com/in/jessicahoganma/">LinkedIn</a></p>
    </div>
	<div class="px-6 pt-12 pb-4 bg-blue-300 text-black">
		@2022 Jessica Hogan
	</div>
</footer>

<style>

	footer a {
		font-weight: bold;
	}
</style>
