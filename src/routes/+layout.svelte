<!-- <script lang="ts">
	import Sidebar from '$lib/components/Sidebar.svelte';
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script> -->

<!-- <svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head> -->

<!-- {@render children()} -->

<!-- <div class="bg-black">
	<main class="">
		{@render children()}
	</main>
</div> -->

<script lang="ts">
	import * as Sidebar from '$lib/components/ui/sidebar/index.js';
	import AppSidebar from '$lib/components/app-sidebar.svelte';
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
	<link
		href="https://fonts.googleapis.com/css2?family=Archivo:ital,wght@0,100..900;1,100..900&family=Mona+Sans:ital,wght@0,200..900;1,200..900&display=swap"
		rel="stylesheet"
	/>
</svelte:head>

<Sidebar.Provider>
	<AppSidebar />
	<main class="h-full">
		<span class="z-10 fixed">
			<Sidebar.Trigger />
		</span>

		{@render children?.()}
	</main>
</Sidebar.Provider>
