<script>
	import Header from '$lib/header/Header.svelte';
	import '../app.css';
</script>

<!-- <Header /> -->

<main>
	<slot />
</main>


<footer class="w-full mx-auto">
	<div class="bg-blue-100 py-12 ">
		<div class="max-w-6xl mx-auto px-6">

			<h2 class="uppercase border-b-2">LinkedIn</h2>
			<p class="py-4">We can get in touch via <a href="https://www.linkedin.com/in/jessicahoganma/">LinkedIn</a></p>
		</div>
	</div>
    <div class=" bg-blue-300">
		<div class="max-w-6xl mx-auto px-6 pb-4 pt-12">
			<div class="text-black">
				@2022 Jessica Hogan
			</div>
		</div>
	</div>
</footer>

<style>

	footer a {
		font-weight: bold;
	}
</style>
