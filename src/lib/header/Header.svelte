<script>
	import Navbar from '$lib/navbar/Navbar.svelte';
	import Sidebar from '$lib/sidebar/Sidebar.svelte';
	import CloudBg from '$lib/img/cloud_bg.png';
	let open = false;
</script>

<section style="background-image: url({CloudBg}); background-position: center; background-repeat: no-repeat; background-size: cover; max-width: 100%; height: 80vh;">
	<Sidebar bind:open/>
	<Navbar bind:sidebar={open}/>
	<div class="hero-text text-white">
		<h1>
			Jessica Hogan
		</h1>
		<p>Data Analyst</p>
	</div>
</section>

<style>
	.hero-text {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 1;
		text-align: center;
		color: var(--tertiary-color);
		height: 70vh;
	}
	h1, p {
		color: inherit;
	}
</style>