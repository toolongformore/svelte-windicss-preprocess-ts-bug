<script lang="ts">
	import { onMount } from 'svelte';

	let content: string;

	onMount(() => {
		content = 'Hello world from Typescript component';
	});
</script>

<div class="bg-green-500">
	{content}. This should be green. But it's not.
</div>
