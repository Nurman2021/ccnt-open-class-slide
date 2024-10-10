<script>
	import { onMount } from 'svelte';
	import Presentation from './Presentation.svelte';

	import Reveal from 'reveal.js';
	import Highlight from 'reveal.js/plugin/highlight/highlight';

	import 'reveal.js/dist/reveal.css';
	import 'reveal.js/dist/theme/night.css';
	import 'reveal.js/plugin/highlight/monokai.css';

	onMount(() => {
		const reveal = new Reveal({
			autoAnimateEasing: 'ease',
			autoAnimateDuration: 1,
			hash: true,
			controls: true,
			progress: true
		});

		reveal.initialize({
			plugins: [Highlight]
		});
	});
</script>

<div class="reveal">
	<div class="slides">
		<Presentation />
	</div>
</div>
