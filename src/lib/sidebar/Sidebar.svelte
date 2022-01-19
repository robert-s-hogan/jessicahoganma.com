<script>
	export let open = false;
</script>

<aside class="absolute w-2/5 h-full bg-gray-300 border-r-2 shadow-lg" class:open>
	<nav class="py-16 px-4 text-xl text-black">
		<a class="block py-2" href="/#about">About</a>
		<a class="block py-2" href="/#services">Services</a>
		<!-- <a class="block py-2" href="/#portfolio">Portfolio</a> -->
		<a class="block py-2" href="/#contact">Contact</a>
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