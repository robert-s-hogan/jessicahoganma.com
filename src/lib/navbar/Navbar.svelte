<script>
	import Hamburger from '$lib/hamburger/Hamburger.svelte'
	import Menu from '$lib/menu/Menu.svelte'
    import Profile from '$lib/img/linkedin_profile.jpeg';
	export let sidebar = false;
</script>



<header class="max-w-6xl mx-auto px-6">
	<div class="flex justify-between py-4 items-center text-black">

		<a href="/">
			<img src="https://rshogan.imgix.net/personal/logos/jh_logo_white.png" alt="Jessica Hogan's Logo" class="h-8" />
		</a>
		<nav class="flex ">
			<div class="hidden md:inline-flex md:flex-end md:space-x-4 text-sm text-black">
				<a class="flex justify-center items-center p-2" href="/#projects">Projects</a>
				<a class="flex justify-center items-center p-2" href="/#who-i-am">Who I Am</a>
				<!-- <a class="flex justify-center items-center py-2" href="/#portfolio">Portfolio</a> -->
				<!-- <a class="flex justify-center items-center py-2" href="/#contact">Contact</a> -->
			</div>
			<Hamburger bind:open={sidebar}/>
			<Menu/>
		</nav>
	</div>

</header>
