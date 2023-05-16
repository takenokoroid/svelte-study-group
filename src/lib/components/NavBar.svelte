<script>
</script>

<div class="wrapper">
	<div class="title">Takeroid Contacts</div>
	<div class="setting-icon">stting icon</div>
	<div class="user-icon">user icon</div>
</div>

<style>
	.wrapper {
		display: grid;
		grid-template-columns: repeat(10, 1fr);
		grid-auto-rows: 100px;
	}

	.title {
		grid-column-start: 1;
		grid-column-end: 2;
		grid-row-start: 1;
		grid-row-end: 2;
	}

	.setting-icon {
		grid-column-start: 9;
		grid-column-end: 10;
		grid-row-start: 1;
		grid-row-end: 2;
	}
	.user-icon {
		grid-column-start: 10;
		grid-column-end: 11;
		grid-row-start: 1;
		grid-row-end: 2;
	}
</style>
