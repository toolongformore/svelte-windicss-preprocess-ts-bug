<script lang="ts">
	import { onMount } from 'svelte';

	let content: string;

	onMount(() => {
		content = 'Hello world from Typescript component (with windi-style-tag)';
	});
</script>

<div class="bg-blue-500">
	{content}. This should be blue. And it is… but only because of the style tag.
</div>

<style windi:preflights:global windi:safelist:global>
</style>
