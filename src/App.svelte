<script>
	import SlotTest from 'slot-test';
	import Baz from './Baz.svelte';

	let show = true;
</script>

<button on:click={()=> show = false}>
	Hide
</button>

<div>
	{#if show }
		<SlotTest>
			<Baz></Baz>
		</SlotTest>
	{/if}
</div>