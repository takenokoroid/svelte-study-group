<script>
	import NavBar from '$lib/components/NavBar.svelte';
	import LeftPane from '$lib/components/LeftPane.svelte';
	import RightPane from '$lib/components/RightPane.svelte';
</script>

<div class="wrapper">
	<div class="navbar-container">
		<NavBar />
	</div>
	<div class="leftpane-container">
		<LeftPane />
	</div>
	<div class="slot-container">
		<slot />
	</div>
	<div class="rightpane-container">
		<RightPane />
	</div>
</div>

<style>
	.wrapper {
		display: grid;
		grid-template-columns: repeat(5, 1fr);
		grid-auto-rows: 100px;
	}

	.navbar-container {
		grid-column-start: 1;
		grid-column-end: 6;
		grid-row-start: 1;
		grid-row-end: 2;
	}

	.leftpane-container {
		grid-column-start: 1;
		grid-row-start: 2;
		grid-row-end: 3;
	}

	.slot-container {
		grid-column-start: 2;
		grid-column-end: 5;
		grid-row-start: 2;
		grid-row-end: 3;
	}

	.rightpane-container {
		grid-column-start: 5;
		grid-column-end: 6;
		grid-row-start: 2;
		grid-row-end: 3;
	}
</style>
