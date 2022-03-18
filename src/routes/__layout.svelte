<script>
	import Header from '$lib/header/Header.svelte';
  import Social from '$lib/social/Social.svelte';
	import '../app.css';
</script>

<Header />

<main>
	<slot />
</main>

<footer class="text-gray-600 body-font">
  <div class="max-w-6xl mx-auto px-6 py-8 flex items-center sm:flex-row flex-col">
    <img src="https://rshogan.imgix.net/personal/logos/jh_logo_white.png" alt="Jessica Hogan's Logo" class="h-8" />
    <p class="text-sm text-gray-500 sm:ml-4 sm:pl-4 sm:border-l-2 sm:border-gray-200 sm:py-2 sm:mt-0 mt-4">© 2022 Jessica Hogan
    </p>
    <Social />
  </div>
</footer>

<style>

	footer a {
		font-weight: bold;
	}


	</style>