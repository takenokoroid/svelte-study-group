<script>
	import ContactCard from '$lib/components/ContactCard.svelte';

	const data = {
		icon: 'icon',
		name: '白瀬咲耶',
		mailAddress: 'aaa@aaa',
		phoneNumber: '090'
	};
</script>

<div class="grid-container">
	<div class="name">名前</div>
	<div class="mail-address">メール</div>
	<div class="phone-number">電話番号</div>
	<div class="contact">連絡先</div>
	<div class="card">
		<ContactCard {...data} />
	</div>
</div>

<style>
	.grid-container {
		display: grid;
		grid-template-columns: repeat(4, 1fr);
		grid-auto-rows: 100px;
	}
	.name {
		grid-column-start: 2;
		grid-column-end: 3;
		grid-row-start: 1;
		grid-row-end: 2;
	}
	.mail-address {
		grid-column-start: 3;
		grid-column-end: 4;
		grid-row-start: 1;
		grid-row-end: 2;
	}
	.phone-number {
		grid-column-start: 4;
		grid-column-end: 5;
		grid-row-start: 1;
		grid-row-end: 2;
	}
	.contact {
		grid-column-start: 1;
		grid-column-end: 5;
		grid-row-start: 2;
		grid-row-end: 3;
	}
	.card {
		grid-column-start: 1;
		grid-column-end: 5;
		grid-row-start: 3;
		grid-row-end: 4;
	}
</style>
