<script lang="ts">
	import { ClipboardCheck, CircleCheckBig, Loader } from 'lucide-svelte';
</script>

<div
	class="w-full p-4 mb-4 text-center bg-white border border-gray-200 rounded-lg shadow-sm sm:p-8 dark:bg-gray-800 dark:border-gray-700"
>
	<h5 class="mb-2 text-xl font-bold text-gray-900 dark:text-white">
		Welcome back 👋 Ready to tackle your tasks today?
	</h5>
	<p class="mb-5 text-base text-gray-500 sm:text-lg dark:text-gray-400">
		Every great achievement starts with a simple to-do. Let's get things done!
	</p>
	<div
		class="items-center justify-center space-y-4 sm:flex sm:space-y-0 sm:space-x-4 rtl:space-x-reverse"
	>
		<div
			class="w-full sm:w-auto bg-gray-800 hover:bg-gray-700 focus:ring-4 focus:outline-none focus:ring-gray-300 text-white rounded-lg inline-flex items-center justify-center px-4 py-2.5 dark:bg-gray-700 dark:hover:bg-gray-600 dark:focus:ring-gray-700"
		>
			<ClipboardCheck class="me-3 w-7 h-7" />
			<div class="text-left rtl:text-right">
				<div class="mb-1 text-xs">Total Tasks</div>
				<div class="-mt-1 font-sans text-sm font-semibold">100</div>
			</div>
		</div>
		<div
			class="w-full sm:w-auto bg-gray-800 hover:bg-gray-700 focus:ring-4 focus:outline-none focus:ring-gray-300 text-white rounded-lg inline-flex items-center justify-center px-4 py-2.5 dark:bg-gray-700 dark:hover:bg-gray-600 dark:focus:ring-gray-700"
		>
			<CircleCheckBig class="me-3 w-7 h-7" />
			<div class="text-left rtl:text-right">
				<div class="mb-1 text-xs">Done Tasks</div>
				<div class="-mt-1 font-sans text-sm font-semibold">100</div>
			</div>
		</div>
		<div
			class="w-full sm:w-auto bg-gray-800 hover:bg-gray-700 focus:ring-4 focus:outline-none focus:ring-gray-300 text-white rounded-lg inline-flex items-center justify-center px-4 py-2.5 dark:bg-gray-700 dark:hover:bg-gray-600 dark:focus:ring-gray-700"
		>
		<Loader class="me-3 w-7 h-7" />
			<div class="text-left rtl:text-right">
				<div class="mb-1 text-xs">Left Tasks</div>
				<div class="-mt-1 font-sans text-sm font-semibold">100</div>
			</div>
		</div>
	</div>
</div>
