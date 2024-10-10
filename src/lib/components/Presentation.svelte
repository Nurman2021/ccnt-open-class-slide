<script>
	import Slide from '$lib/components/Slide.svelte';
	import Code from './Code.svelte';
	import Indigo from '$lib/images/indigohub.png';
	import Svelte from '$lib/images/svelte.png';
	import coconut from '$lib/images/coconut.png';
	import Meme from '$lib/images/meme.jpg';
</script>

<Slide>
	<div class="flex justify-center">
		<img src={Svelte} alt="logo svelte" class="mb-8 h-44" />
	</div>
	<h3>THE FRONTEND FRAMEWORK OF THE FUTURE</h3>
	<small>Presentation by <a href="/nurman">Nurman Awaluddin</a></small>
	<div class="flex items-center justify-center gap-4 border-t border-gray-400">
		<small class="text-2xl text-white">Sponsored by</small>
		<img src={coconut} alt="" class="h-20" />
		<img src={Indigo} alt="" class="h-20" />
	</div>
</Slide>

<Slide>
	<p class="text-white">WHAT is Svelte ?</p>
</Slide>

<Slide>
	<p class="text-white">Svelte Comparation</p>
</Slide>

<Slide>
	<p class="text-white">Svelte Feature</p>
</Slide>

<Slide>
	<Slide>
		<p class="text-white">How to Start Svelte?</p>
	</Slide>
	<Slide>
		<p class="text-white">apa itu?</p>
	</Slide>
	<Slide>
		<Code>
			{`
			function fly(){
			
			}
			`}
		</Code>
	</Slide>
</Slide>

<Slide>
	<p class="text-white">Lets Code!!</p>
	<div class="flex justify-center">
		<img src={Meme} alt="" />
	</div>
</Slide>

<Slide>
	<p class="text-white">ANY QUESTION?</p>
</Slide>
