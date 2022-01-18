<script>
	import { onMount } from 'svelte';

	import screenshot from '../assets/screenshot-vite-static-typography-build.png';

	let content;

	onMount(() => {
		content = 'Hello world from Javascript typography';
	});
</script>

<div class="prose">
	<h3>{content}</h3>
	<p>
		This should be prose. And it is (if you don't mind the vite <code>Unused CSS selector</code> warnings).
	</p>
	<p>But… oh no! It can no longer be build with the static adapter:</p>
	<img src={screenshot} alt="" />
</div>
