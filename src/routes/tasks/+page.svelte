<script lang="ts">
	import Table from './Table.svelte';


</script>

<div class="p-5 sm:ml-64">
	<div class="p-4 mt-14">
		<div class="relative overflow-x-auto shadow-md sm:rounded-lg">
			<table class="w-full text-sm text-left rtl:text-right text-gray-500 dark:text-gray-400">
				<thead
					class="text-xs text-gray-700 uppercase bg-gray-50 dark:bg-gray-700 dark:text-gray-400"
				>
					<tr>
						<th scope="col" class="px-6 py-3"> Task Name </th>
						<th scope="col" class="px-6 py-3"> Status </th>
						<th scope="col" class="px-6 py-3"> Category </th>
						<th scope="col" class="px-6 py-3"> Edit</th>
					</tr>
				</thead>
				<tbody>
					<Table data={{id: 1, title: 'Apple MacBook Pro 17"', status: true, category: 'Laptop'}} />
					<Table data={{id: 2, title: 'Apple MacBook Pro 17"', status: true, category: 'Laptop'}} />
					<Table data={{id: 3, title: 'Apple MacBook Pro 17"', status: false, category: 'Laptop'}} />
					<Table data={{id: 4, title: 'Apple MacBook Pro 17"', status: false, category: 'Laptop'}} />
					<Table data={{id: 5, title: 'Apple MacBook Pro 17"', status: false, category: 'Laptop'}} />
					<Table data={{id: 6, title: 'Apple MacBook Pro 17"', status: true, category: 'Laptop'}} />

				</tbody>
			</table>
		</div>
	</div>
</div>
