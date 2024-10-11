<script>
	import Slide from '$lib/components/Slide.svelte';
	import Code from './Code.svelte';
	import Indigo from '$lib/images/indigohub.png';
	import Svelte from '$lib/images/svelte.png';
	import coconut from '$lib/images/coconut.png';
	import Meme from '$lib/images/meme.jpg';
	import Demo from '$lib/images/todo.png';
	import Bundle from '$lib/images/library_size.png';
	import ReactCode from '$lib/images/react_code.png';
	import SvelteCode from '$lib/images/svelte_code.png';
	import ReactRoute from '$lib/images/react_route.png';
	import SvelteRoute from '$lib/images/svelte_route.png';

	// import Terminal from '$lib/demo.mkv';
	import Me from '$lib/images/my-photo.jpg';
</script>

<Slide>
	<div class="flex justify-center">
		<img src={Svelte} alt="logo svelte" class="mb-8 h-44" />
	</div>
	<h3>THE FRONTEND FRAMEWORK OF THE FUTURE</h3>
	<small>Presentation by <a href="https://noorman.vercel.app/">Nurman Awaluddin</a></small>
	<div class="flex items-center justify-center gap-4 border-t border-gray-400">
		<small class="text-2xl text-white">Supported by</small>
		<img src={coconut} alt="" class="h-20" />
		<img src={Indigo} alt="" class="h-20" />
	</div>
</Slide>
<Slide>
	<Slide>
		<p>WHAT is <strong>Svelte</strong> ?</p>
	</Slide>
	<Slide>
		<p>
			<strong>Svelte</strong> adalah sebuah compiler yang menghasilkan kode JavaScript yang minimal
			dan sangat dioptimalkan dari kode komponen yang kita tulis <br /> <br /> <br />
			<small>Sumber: MDN Web Docs</small>
		</p>
	</Slide>
</Slide>

<Slide>
	<Slide>
		<p class="text-white">Svelte Comparation</p>
	</Slide>
	<Slide>
		<p>Ukuran Paket yang Digunakan</p>
		<div class="flex justify-center">
			<img src={Bundle} alt="" />
		</div>
	</Slide>
	<Slide animate>
		<p class="text-blue-600">Perbandingan Kode</p>
		<div class="flex justify-center">
			<img src={ReactCode} alt="" />
		</div>
	</Slide>
	<Slide animate>
		<p class="text-orange-500">Perbandingan Kode</p>
		<div class="flex justify-center">
			<img src={SvelteCode} alt="" />
		</div>
	</Slide>
	<Slide animate>
		<p class=" text-blue-600">Routing</p>
		<div class="flex justify-center">
			<img src={ReactRoute} alt="" class=" max-h-screen" />
		</div>
	</Slide>
	<Slide animate>
		<p class=" text-orange-500">Routing</p>
		<div class="flex justify-center">
			<img src={SvelteRoute} alt="" class="h-4/5" />
		</div>
	</Slide>
</Slide>
<Slide>
	<Slide>
		<p class="text-white">Svelte Feature</p>
	</Slide>
	<Slide>
		<ul>
			<li>Ukuran Kode yang <strong>Kecil</strong></li>
			<li>Efisiensi Runtime</li>
			<li>Kode yang Sederhana dan Bersih</li>
			<li>Reaktivitas Bawaan</li>
			<li>Progressive Enhancement</li>
		</ul>
	</Slide>
	<Slide>
		<div class="flex justify-center">
			<img src={Me} alt="" class=" h-4/5" />
		</div>
	</Slide>
	<!-- <Slide>
		<video src={Terminal} autoplay></video>
	</Slide> -->
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
			npm create svelte@latest

			npx svelte-add tailwindcss


			`}
		</Code>
	</Slide>
</Slide>
<Slide>
	<Slide>
		<p>Lets Code!!</p>

		<div class="flex justify-center">
			<img src={Meme} alt="" />
		</div>
	</Slide>
	<Slide>
		<h4 class="text-white">Todo List App</h4>
		<div class="flex justify-center">
			<img src={Demo} alt="" />
		</div>
	</Slide>
</Slide>

<Slide>
	<p class="text-white">ANY QUESTION?</p>
</Slide>
