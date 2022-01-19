<script>
	import Hamburger from '$lib/hamburger/Hamburger.svelte'
	import Menu from '$lib/menu/Menu.svelte'
    import Profile from '$lib/img/linkedin_profile.jpeg';
	export let sidebar = false
</script>

<header class="flex justify-between p-4 items-center text-white">
	<a href="/"><p class="text-white">JH</p></a>
	<nav class="flex ">
		<Hamburger bind:open={sidebar}/>
	</nav>
	<Menu/>
</header>