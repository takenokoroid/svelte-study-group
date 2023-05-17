<script>
	/** @type {string} */
	export let icon;
	/** @type {string} */
	export let name;
	/** @type {string} */
	export let mailAddress;
	/** @type {string} */
	export let phoneNumber;
</script>

<div class="flex-container">
	<div>{icon}</div>
	<div>{name}</div>
	<div>{mailAddress}</div>
	<div>{phoneNumber}</div>
</div>

<style>
	.flex-container {
		display: flex;
		flex-direction: row;
		justify-content: space-between;
	}
</style>
