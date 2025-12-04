<script>
	import { AspectRatio } from '$lib/components/ui/aspect-ratio/index.js';
	import { Badge } from '$lib/components/ui/badge/index.js';
	import * as Empty from '$lib/components/ui/empty/index.js';
	// import FolderCodeIcon from "@tabler/icons-svelte/icons/folder-code";
    import * as Breadcrumb from "$lib/components/ui/breadcrumb/index.js";
</script>

<section class="pp-content p-16 py-24 h-full overflow-y-hidden">
	<section class="pp-thumbnail-img flex flex-col gap-4 mb-12">
		<img
			class="project-thumbnail mb-1 rounded-xl border-2  "
			src="/media/general/coming-soon.webp"
			alt="Bankment: A Stellar New Year Project Thumbnail"
		/>
        <h1 class="scroll-m-20 text-4xl font-extrabold tracking-tight lg:text-5xl">
			(WIP) Bankment: A Stellar New Year
		</h1>
        <div class="flex flex-row">
            <Badge variant="outline">Product Design</Badge>
        </div>
	</section>
</section>