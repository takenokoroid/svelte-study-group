<script>
	import NavBar from '$lib/components/NavBar.svelte';
	import SideBar from '$lib/components/SideBar.svelte';
</script>

<div class="wrapper">
	<div class="box1">
		<NavBar />
	</div>
	<div class="box2">
		<SideBar />
	</div>
	<div class="box3">
		<slot />
	</div>
</div>

<style>
	.wrapper {
		display: grid;
		grid-template-columns: repeat(4, 1fr);
		grid-auto-rows: 100px;
	}

	.box1 {
		grid-column-start: 1;
		grid-column-end: 5;
		grid-row-start: 1;
		grid-row-end: 2;
	}

	.box2 {
		grid-column-start: 1;
		grid-row-start: 2;
		grid-row-end: 3;
	}

	.box3 {
		grid-column-start: 2;
		grid-column-end: 5;
		grid-row-start: 2;
		grid-row-end: 3;
	}
</style>
