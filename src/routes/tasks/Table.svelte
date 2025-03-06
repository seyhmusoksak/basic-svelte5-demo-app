<script lang="ts">
	interface tableData {
		id: number;
		title: string;
		status: boolean;
		category: string;
	}

	export let data: tableData;
</script>

<tr
	class="bg-white border-b dark:bg-gray-800 dark:border-gray-700 border-gray-200 hover:bg-gray-50 dark:hover:bg-gray-600"
>
	<th scope="row" class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap dark:text-white">
		{data.title}
	</th>
	<td class="px-6 py-4">
		<label class="inline-flex items-center cursor-pointer">
		  <input type="checkbox" value="" class="sr-only peer" checked={data.status}>
		  <div class="relative w-11 h-6 bg-gray-200 rounded-full peer peer-focus:ring-4 peer-focus:ring-blue-300 dark:peer-focus:ring-blue-800 dark:bg-gray-700 peer-checked:after:translate-x-full rtl:peer-checked:after:-translate-x-full peer-checked:after:border-white after:content-[''] after:absolute after:top-0.5 after:start-[2px] after:bg-white after:border-gray-300 after:border after:rounded-full after:h-5 after:w-5 after:transition-all dark:border-gray-600 peer-checked:bg-blue-600 dark:peer-checked:bg-blue-600"></div>
		</label>
	</td>
	<td class="px-6 py-4"> {data.category} </td>
	<td class="px-6 py-4"> <span class="text-underline text-blue-700">Edit</span> </td>
</tr>
