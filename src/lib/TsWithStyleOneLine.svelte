<script lang="ts">
	import { onMount } from 'svelte';
	import screenshot1 from '../assets/screenshot-vscode-1.png';
	import screenshot2 from '../assets/screenshot-vscode-2.png';

	let content: string;

	onMount(() => {
		content = 'Hello world from Typescript component (with one-line windi-style-tag)';
	});
</script>

<div class="bg-lime-500">
	{content}. This should be lime. And it is… but the style-tag where opening and closing tags are
	one line shows errors (in VSCode):
	<img src={screenshot1} alt="" class="h-24 mb-1" />
	<img src={screenshot2} alt="" class="h-24" />
</div>

<style windi:preflights:global windi:safelist:global></style>
