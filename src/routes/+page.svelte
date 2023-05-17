<script>
	import ContactCard from '$lib/components/ContactCard.svelte';

	const data = {
		icon: 'icon',
		name: '白瀬咲耶',
		mailAddress: 'aaa@aaa',
		phoneNumber: '090'
	};
</script>

<div class="flex-container">
	<div>名前</div>
	<div>メール</div>
	<div>電話番号</div>
</div>

<div class="box">
	<div>連絡先</div>
	<ContactCard {...data} />
</div>

<style>
	.flex-container {
		display: flex;
		flex-direction: row;
		justify-content: space-between;
	}
</style>
