<script>
	import Hamburger from '$lib/hamburger/Hamburger.svelte'
	import Menu from '$lib/menu/Menu.svelte'
    import Profile from '$lib/img/linkedin_profile.jpeg';
	export let sidebar = false
</script>

<header class="max-w-6xl mx-auto px-6">
	<div class="flex justify-between p-4 items-center text-black">

		<a href="/"><p class="text-black text-2xl">JH</p></a>
		<nav class="flex ">
			<Hamburger bind:open={sidebar}/>
		</nav>
		<Menu/>
	</div>
</header>

<style>
	header {
		height: 10vh;
	}
</style>