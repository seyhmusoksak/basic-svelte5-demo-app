<script lang="ts">
	import Card from './MyCard.svelte';
	const data = [
	{
		id: 1,
		title: 'Total Tasks',
		total: 10,
		done: 5,
	},
	{
		id: 2,
		title: 'Completed Tasks',
		total: 5,
		done: 2,
	},
	{
		id: 3,
		title: 'Pending Tasks',
		total: 5,
		done: 3,
	},
	{
		id: 4,
		title: 'Overdue Tasks',
		total: 5,
		done: 0,
	},
	];
</script>


<div class="p-5 sm:ml-64">
	<div class="p-4 mt-14">
		<div class="grid grid-cols-4 gap-3 mb-4">
			{#each data as item}
				<Card data={item}/>
			{/each}
		</div>
	</div>
</div>
