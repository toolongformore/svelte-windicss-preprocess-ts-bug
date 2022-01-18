<script>
	import { onMount } from 'svelte';

	let content;

	onMount(() => {
		content = 'Hello world from Javascript component';
	});
</script>

<div class="bg-red-500">
	{content}. This should be red. And it is.
</div>
