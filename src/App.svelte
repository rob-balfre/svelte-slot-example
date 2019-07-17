<script>
	import SlotTest from 'slot-test';
	import Baz from './Baz.svelte';

	let bookings = ['one', 'two', 'three'];

	function handleEmpty() {
		bookings = []
	}
</script>

<button on:click={handleEmpty}>
	Empty bookings
</button>

{#each bookings as booking}
<SlotTest>
	<Baz></Baz>
</SlotTest>
{/each}