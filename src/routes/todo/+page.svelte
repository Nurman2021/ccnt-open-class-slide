<script>
	import '../../app.css';
</script>

<svelte:head>
	<title>Simple Todo</title>
	<meta name="description" content="Coconut Open Class" />
</svelte:head>
<main class="h-screen bg-orange-100">
	<section class="mx-auto max-w-[700px] border border-black px-3">
		<!-- input -->
		<h1 class="my-6 text-center text-3xl font-bold">
			Todo<span class="text-green-300">List</span>
		</h1>
		<div class="flex gap-2 px-3">
			<input
				type="text"
				class="w-full rounded-full border-2 border-black bg-orange-200"
				placeholder="Masukkan kegiatan"
			/>
			<button class="h-16 w-16 rounded-full bg-black font-bold text-white">Add</button>
		</div>

		<!-- todo container -->
		<div class="mt-6 border-t-2 border-gray-400 p-3">
			<div class="flex h-20 items-center gap-2 rounded-xl border-2 border-black bg-blue-400 px-3">
				<input type="checkbox" />
				<h4>Programming</h4>
				<div>
					<button>Save</button>
					<button>Edit</button>
				</div>
			</div>
		</div>
	</section>
</main>
