<script lang="ts">
	import { onMount } from 'svelte';
	import Card from './MyCard.svelte';
	import Banner from './Banner.svelte';

	type Task = {
		id: number;
		title: string;
		total: number;
		done: number;
	};

	let tasks: Task[];

	const url = 'http://localhost:8080/products';

	onMount(async () => {
		fetch(url)
			.then((response) => response.json())
			.then((data) => {
				tasks = data;
			});
	});
</script>

<div class="p-5 sm:ml-64">
	<div class="p-4 mt-14">
		<Banner />

		<div class="grid grid-cols-1 md:grid-cols-3 gap-3 mb-4">
			{#each tasks as item}
				<Card data={item} />
			{/each}
		</div>
	</div>
</div>
