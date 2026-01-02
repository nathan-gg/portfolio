<script>
	import { AspectRatio } from '$lib/components/ui/aspect-ratio/index.js';
	import { Badge } from '$lib/components/ui/badge/index.js';
	import * as Empty from '$lib/components/ui/empty/index.js';
	// import FolderCodeIcon from "@tabler/icons-svelte/icons/folder-code";
</script>

<section class="home-content p-16 py-24 h-full overflow-y-hidden w-full flex flex-col items-center">
	<section
		class="flex flex-col 2xl:flex-row h-fit gap-4 lg:gap-8 mb-6 pb-6 border-b border-b-border w-full 2xl:w-4/5 justify-between"
	>
		<div class="bio flex flex-col gap-4">
			<span class="flex flex-row gap-2">
				<h1 class="scroll-m-20 text-4xl font-extrabold tracking-tight lg:text-5xl mb-0">
					Nathan Gebreab
				</h1>
			</span>

			<h2 class="scroll-m-20 mt-0 text-2xl text-muted-foreground font-semibold tracking-tight">
				Front-End Web Developer & UI/UX Designer
			</h2>
			<p class="bio-text max-w-160">
				Hello! I am a <span class="font-bold">UI/UX Designer</span> and <span class="font-bold">Front-End Web Developer</span> based in Vancouver, British
				Columbia, Canada, and currently pursuing an Interactive Arts and Technology BSc at Simon
				Fraser University. I love creating unique digital experiences for users and
				<span class="font-bold">sparking creativity</span> through each and every interaction!
			</p>
		</div>

		<div class="flex flex-col md:flex-row h-fit">
			<img
				class="bio-photo rounded-xl h-64 object-cover"
				src="/media/general/about-headshot.webp"
				alt="Nathan Gebreab"
			/>
		</div>
	</section>

	<section class="project-feed flex flex-col w-full md:w-4/5">
		<h2
			class="pb-2 text-3xl mb-4 font-semibold tracking-tight transition-colors first:mt-0"
		>
			Projects
		</h2>
		<div class="flex flex-col 2xl:flex-row justify-between gap-8">
			<a href="/projects/green-basil" class="hover:border-chart-2">
				<img
					class="project-thumbnail mb-2 rounded-xl border-white border-2"
					src="/media/green-basil/gb-thumbnail.webp"
					alt="Green Basil Thai Restaurant Project Thumbnail"
				/>
				<div class="flex flex-row justify-between">
					<h3 class="project-title scroll-m-20 text-xl font-semibold tracking-tight">
						Green Basil Thai Restaurant
					</h3>
					<p class="project-date text-muted-foreground">2025</p>
				</div>
				<Badge variant="outline" class="text-muted-foreground">Lead Front-End</Badge>
				<p class="project-brief">A modernized website for a Metro Vancouver staple.</p>
			</a>
			<!-- <a href="/projects/industry-media" class="*:hover:border-chart-1">
				<img
					class="project-thumbnail mb-2 rounded-xl border-white border-2"
					src="/media/general/coming-soon.webp"
					alt="Project Coming Soon!"
				/>
				<div class="flex flex-row justify-between">
					<h3 class="project-title scroll-m-20 text-xl font-semibold tracking-tight">
						(WIP) Industry Media Group
					</h3>
					<p class="project-date text-muted-foreground">2025</p>
				</div>
				<Badge variant="outline" class="text-muted-foreground">Junior Front-End</Badge>
				<p class="project-brief"></p>
			</a>
			<a href="/projects/mosaic" class="*:hover:border-chart-1">
				<img
					class="project-thumbnail mb-2 rounded-xl border-white border-2"
					src="/media/general/coming-soon.webp"
					alt="Project Coming Soon!"
				/>
				<div class="flex flex-row justify-between">
					<h3 class="project-title scroll-m-20 text-xl font-semibold tracking-tight">
						(WIP) Mosaic: Event App
					</h3>
					<p class="project-date text-muted-foreground">2025</p>
				</div>
				<Badge variant="outline" class="text-muted-foreground">UI/UX Design / Motion Graphics</Badge
				>
				<p class="project-brief"></p>
			</a>
			<a href="/projects/bankment-stellar" class="*:hover:border-chart-1">
				<img
					class="project-thumbnail mb-2 rounded-xl border-white border-2"
					src="/media/general/coming-soon.webp"
					alt="Project Coming Soon!"
				/>
				<div class="flex flex-row justify-between">
					<h3 class="project-title scroll-m-20 text-xl font-semibold tracking-tight">
						(WIP) Bankment: A Stellar New Year
					</h3>
					<p class="project-date text-muted-foreground">2025</p>
				</div>
				<Badge variant="outline" class="text-muted-foreground">Product Design</Badge>
				<p class="project-brief"></p>
			</a> -->
		</div>
	</section>
</section>
