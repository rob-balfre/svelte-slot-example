<script>
	import Baz from 'fake-component-lib/Baz';
	
	let show = true;
</script>

<button on:click={()=> show = false}>
	Hide
</button>

<div>
	{#if show }
		<Baz></Baz>
	{/if}
</div>