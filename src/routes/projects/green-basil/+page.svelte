<script>
	import { AspectRatio } from '$lib/components/ui/aspect-ratio/index.js';
	import { Badge } from '$lib/components/ui/badge/index.js';
	import * as Empty from '$lib/components/ui/empty/index.js';
	// import FolderCodeIcon from "@tabler/icons-svelte/icons/folder-code";
	import * as Breadcrumb from '$lib/components/ui/breadcrumb/index.js';
</script>

<section class="pp-content p-16 py-24 h-full overflow-y-hidden">
	<section class="pp-thumbnail-img flex flex-col gap-4 mb-12">
		<img
			class="project-thumbnail mb-1 rounded-xl border-2"
			src="/media/green-basil/gb-thumbnail.webp"
			alt="Green Basil Thai Restaurant Project Thumbnail"
		/>
		<h1 class="scroll-m-20 text-4xl font-extrabold tracking-tight lg:text-5xl">
			Green Basil Thai Restaurant
		</h1>
		<div class="flex flex-row">
			<Badge variant="outline">Lead Web Developer</Badge>
		</div>
	</section>
	<section class="pp-header mb-12">
		<div class="pp-details mb-4">
			<h2 class="scroll-m-20 mt-0 text-2xl font-semibold tracking-tight">Details</h2>
			<ul class=" ms-6 list-disc [&>li]:mt-2">
				<li>Duration: March 2025 - May 2025</li>
				<li>
					See the finished project here: <a
						class="text-chart-3 hover:underline"
						target="_blank"
						href="https://greenbasilrestaurant.ca/">greenbasilrestaurant.ca</a
					>
				</li>
				<li>Role: Lead Developer</li>
				<li>Skills: Svelte, Figma, HTML, CSS, JavaScript</li>
				<li>
					Team Members: Ethan Li (UX/UI), Tirsten Lisondra (UX/UI), Max Li (Project Supervisor)
				</li>
			</ul>
		</div>
		<div class="pp-desc mb-4">
			<h2 class="scroll-m-20 mt-0 text-2xl font-semibold tracking-tight">Overview</h2>
			<p>
				Green Basil Thai Restaurant is located in Burnaby, BC, and has been a cornerstone of Thai
				cuisine since 2006. For this project, our team was tasked with redesigning and modernizing
				their website to appeal to a new generation of customers.
			</p>
		</div>
		<div class="pp-goals mb-4">
			<h2 class="scroll-m-20 mt-0 text-2xl font-semibold tracking-tight">My Goals</h2>
			<p>
				In this project, my goal was to develop a website that was both functional and easy to use.
				Additionally, as we were not given a concrete deadline for the project, I took my time to
				learn as many new skills as possible, including how to use the UI framework known as Svelte.
			</p>
		</div>
	</section>
	<section class="pp-process mb-12">
		<div>
			<h2 class="scroll-m-20 mt-0 text-2xl font-semibold tracking-tight">Process</h2>
			<h3 class="scroll-m-20 text-xl font-semibold tracking-tight">Stage 1: Making a Plan</h3>
			<p>
				My goal for this project was to approach it with a learn-first mentality. I spent the
				initial stages of the project reading the Svelte Documentation and familiarizing myself with
				its features, allowing me to better understand web interactions and explain to the design
				team how I would implement their ideas.
			</p>
		</div>

		<div>
			<h3 class="scroll-m-20 text-xl font-semibold tracking-tight">Stage 2: Development</h3>
			<p>
				In the working process, I focused on constantly testing responsiveness, link validity, and
				interaction design, etc., to achieve the desired results. Additionally, I adopted a rigid
				schedule to keep myself on task and ensure that progress was always being made.
			</p>
			<video
				class="case-media my-6 rounded-xl border-2"
				width="1458"
				height="830"
				autoplay
				loop
				muted
			>
				<source src="/media/green-basil/portfolio-gb-responsiveness.mp4" />
			</video>
		</div>

		<div>
			<h3 class="scroll-m-20 text-xl font-semibold tracking-tight">Stage 3: Reflection</h3>
			<p>
				The struggle: As a first-time solo developer working with a lesser-known framework like
				Svelte, debugging was a tedious process. An instance of this was an issue with the
				snap-scrolling effect on certain pages, where the overflow margins would be incorrect, or
				other features would no longer function.
			</p>
			<p>
				The solution: While the fix ended up being a simple CSS error, an important thing that this
				taught me was to re-evaluate and come back to a problem with a different mindset. Instead of
				getting stuck on this one bug, I was able to be productive in other areas and develop
				separate skills, so that by the time this bug resurfaced to the top of my to-do list, I was
				ready to tackle it.
			</p>
			<video
				class="case-media my-6 rounded-xl border-2"
				width="1904"
				height="944"
				autoplay
				loop
				muted
			>
				<source src="/media/green-basil/portfolio-gb-scrollsnap.mp4" />
			</video>
		</div>

		<div>
			<h3 class="scroll-m-20 text-xl font-semibold tracking-tight">Stage 4: Going Forward</h3>
			<h4 class="scroll-m-20 text-lg font-semibold tracking-tight">What I Would do Different</h4>
			<p>
				One of the main things I learned was the importance of web scaffolding. If I were to do this
				project again, rather than planning along the way, I would first collect all the data I
				need, organize it into JavaScript files that have the parameters of the data sorted into the
				groups needed, and then begin the HTML and CSS.
			</p>
			<h4 class="scroll-m-20 text-lg font-semibold tracking-tight">What I Learned</h4>
			<p>
				I gained many skills throughout this project, most significantly working within Svelte, a UI
				framework, for the first time. I learned about the importance of proper scaffolding, the
				length of the iterative process and debugging, and how to keep a consistent work schedule to
				keep a team motivated.
			</p>
		</div>
	</section>
</section>
