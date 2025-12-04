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
