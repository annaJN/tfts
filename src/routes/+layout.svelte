<script lang="ts">
	import '../app.css';
	const tabs = ['Hem', 'Vison', 'Praktiskt'];
</script>

<header class="bg-teal-300 h-10" />

<img
	src="/img/tftsLogga.png"
	alt="Tales from the sprawl using a purple, pink and teal dragon with a skull for a head as the s in Sprawl"
/>
<nav class="mx-auto max-w-prose">
	<ul class="flex flex-wrap text-sm font-medium text-center text-gray-500 border-b border-gray-200">
		{#each tabs as tab}
			<li class="mr-2">
				<a
					href="#"
					class="inline-block p-4 text-blue-600 bg-teal-100 rounded-t-lg dark:bg-gray-800 dark:text-blue-500"
					>{tab}</a
				>
			</li>
		{/each}

		<li class="mr-2">
			<a
				href="#"
				class="inline-block p-4 rounded-t-lg border-4 border-teal-400 hover:text-gray-600 hover:bg-gray-50"
				>Dashboard</a
			>
		</li>
	</ul>
</nav>

<slot />

<footer class="bg-amber-400 px-3 py-4">
	<p class="font-bold">Designed by nill</p>
</footer>
