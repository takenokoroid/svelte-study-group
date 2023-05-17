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

<div class="contact-card-grid">
	<div>{icon}</div>
	<div>{name}</div>
	<div>{mailAddress}</div>
	<div>{phoneNumber}</div>
</div>

<style>
	.contact-card-grid {
		display: grid;
		grid-template-columns: repeat(4, 1fr);
		grid-auto-rows: 100px;
	}
</style>
