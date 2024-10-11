<script>
	import '../../app.css';

	import { Trash2 } from 'lucide-svelte';
	import { Pencil } from 'lucide-svelte';
	import { Save } from 'lucide-svelte';
	import { Plus } from 'lucide-svelte';

	let toDolist = [];
	let textInput = '';

	function addTodo() {
		toDolist = [...toDolist, { content: textInput, editing: false }];
	}

	function deleteTodo(i) {
		toDolist.splice(i, 1);
		toDolist = toDolist;
	}

	function editTodo(i, isEdit) {
		toDolist[i].editing = isEdit;
	}
</script>

<svelte:head>
	<title>Simple Todo</title>
	<meta name="description" content="Coconut Open Class" />
</svelte:head>
<main class="h-screen bg-orange-100 py-4">
	<section class="mx-auto h-full max-w-[700px] overflow-auto rounded-lg border border-black px-3">
		<!-- input -->
		<h1 class="my-6 text-center text-3xl font-bold">
			Todo<span class="text-green-300">List</span>
		</h1>
		<div class="flex gap-2 px-3">
			<input
				type="text"
				class="w-full rounded-full border-2 border-black bg-orange-200 px-3"
				placeholder="Masukkan kegiatan"
				bind:value={textInput}
			/>
			<button
				class="rounded-full bg-black p-4 font-bold text-white hover:bg-gray-500"
				on:click={addTodo}><Plus /></button
			>
		</div>

		<!-- todo container -->
		<div class="mt-6 space-y-3 border-t-2 border-gray-400 p-3">
			{#each toDolist as todo, i}
				<div
					class="flex h-16 items-center justify-between gap-2 rounded-xl border-2 border-black bg-blue-400 px-3"
				>
					{#if todo.editing}
						<input type="text" bind:value={todo.content} class="w-full rounded-full px-3" />
					{:else}
						<input type="checkbox" />
						<p class="text-lg font-semibold capitalize">{todo.content}</p>
					{/if}
					<div class="flex gap-2">
						{#if todo.editing}
							<button on:click={() => editTodo(i, false)}><Save /></button>
						{:else}
							<button on:click={() => editTodo(i, true)}><Pencil /></button>
						{/if}
						<button class="hover:text-red-600" on:click={() => deleteTodo(i)}><Trash2 /></button>
					</div>
				</div>
			{/each}
		</div>
	</section>
</main>
