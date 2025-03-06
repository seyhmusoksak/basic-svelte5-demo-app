<script>
	import Card from './Mycard.svelte';
	const data = [
	{
		title: 'Total Tasks',
		total: 10,
		done: 5,
	},
	{
		title: 'Completed Tasks',
		total: 5,
		done: 2,
	},
	{
		title: 'Pending Tasks',
		total: 5,
		done: 3,
	},
	{
		title: 'Overdue Tasks',
		total: 5,
		done: 0,
	},
	];
</script>


<div class="p-5 sm:ml-64">
	<div class="p-4 mt-14">
		<div class="grid grid-cols-3 gap-4 mb-4">
			{#each data as item}
				<Card data={item}/>
			{/each}
		</div>
	</div>
</div>
