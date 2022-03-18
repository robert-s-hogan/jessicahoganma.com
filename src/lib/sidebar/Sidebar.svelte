<script>
	export let open = false;
</script>

<aside class={open ? `absolute lg:hidden w-full h-2/5 justify-center items-center text-center bg-gray-300 border-r-2 shadow-lg bg-white` : 'hidden'} class:open>
	<nav class="py-16 px-4 text-xl text-black grid grid-cols-1">
		<a class="flex justify-center items-center p-2" href="/#projects">Projects</a>
		<a class="flex justify-center items-center p-2" href="/#who-i-am">Who I Am</a>
		<!-- <a class="flex justify-center items-center py-2" href="/#portfolio">Portfolio</a> -->
		<a class="flex justify-center items-center py-2" href="/#contact">Contact</a>
	</nav>
</aside>

<style>
	aside {
		right: -100%;
		transition: right 0.3s ease-in-out
	}
	
	.open {
		right: 0
	}

	nav a {
		color: inherit;
	}
</style>