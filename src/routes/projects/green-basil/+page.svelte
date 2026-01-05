<script>
	import { AspectRatio } from '$lib/components/ui/aspect-ratio/index.js';
	import { Badge } from '$lib/components/ui/badge/index.js';
	import * as Empty from '$lib/components/ui/empty/index.js';
	import ArrowLeft from '@lucide/svelte/icons/arrow-left';
	import Clock from '@lucide/svelte/icons/clock';
	import Users from '@lucide/svelte/icons/users';
	import SquareUser from '@lucide/svelte/icons/square-user';
	import ExternalLink from '@lucide/svelte/icons/external-link';
	import Ruler from '@lucide/svelte/icons/ruler';
	// import FolderCodeIcon from "@tabler/icons-svelte/icons/folder-code";
	import * as Breadcrumb from '$lib/components/ui/breadcrumb/index.js';

	import { onMount } from 'svelte';

	onMount(() => {
		document.body.style.backgroundColor = '#f3fff4';

		return () => {
			document.body.style.backgroundColor = ''; // cleanup
		};
	});
</script>

<section class="pp-content p-16 pb-24 pt-12 h-full overflow-y-hidden w-full">
	<a href="/" class="flex flex-row gap-1 mb-12"><ArrowLeft />Back to Home Page</a>
	<section class="pp-thumbnail-img flex flex-col gap-4 mt-6 md:mt-12 mb-12">
		<!-- <h1 class="scroll-m-20 text-4xl font-extrabold tracking-tight lg:text-5xl">
			Green Basil Thai Restaurant
		</h1> -->
		<!-- <div class="flex flex-row">
			<Badge variant="outline">Lead Web Developer</Badge>
		</div> -->
		<div class="flex flex-col 2xl:flex-row gap-1 justify-between w-full">
			<h1 class="scroll-m-20 text-4xl font-extrabold tracking-tight lg:text-5xl">
				Green Basil Thai Restaurant
			</h1>
			<div class="pp-details mb-4 w-fit">
				<!-- <h2 class="scroll-m-20 mt-0 text-2xl font-semibold tracking-tight">Details</h2> -->
				<!-- <ul class=" ms-6 list-disc [&>li]:mt-2">
					<li>Duration: March 2025 - May 2025</li>
					<li>
						See the finished project here: <a
							class="text-chart-2 hover:underline"
							target="_blank"
							href="https://greenbasilrestaurant.ca/">greenbasilrestaurant.ca</a
						>
					</li>
					<li>Role: Lead Developer</li>
					<li>Skills: Svelte, Figma, HTML, CSS, JavaScript</li>
					<li>
						Team Members: Ethan Li (UX/UI), Tirsten Lisondra (UX/UI), Max Li (Project Supervisor)
					</li>
				</ul> -->
			</div>
		</div>
		<div class="flex flex-col lg:flex-row gap-2 justify-start w-full flex-wrap">
			<div class="border-2 border-[#82df9e] rounded-lg p-4 bg-white w-full lg:w-fit">
				<div class="flex flex-row gap-1 items-center mb-2">
					<Clock color="#82df9e" />
					<h2 class="scroll-m-20 mt-0 text-xl font-semibold tracking-tight w-fit">Duration</h2>
				</div>

				<p class="text">March 2025 - May 2025</p>
			</div>

			<div class="border-2 border-[#82df9e] rounded-lg p-4 bg-white w-full lg:w-fit">
				<div class="flex flex-row gap-1 items-center mb-2">
					<SquareUser color="#82df9e" />
					<h2 class="scroll-m-20 mt-0 text-xl font-semibold tracking-tight w-fit">Role</h2>
				</div>

				<p class="text">Lead Developer</p>
			</div>
			<div class="border-2 border-[#82df9e] rounded-lg p-4 bg-white w-full lg:w-fit">
				<div class="flex flex-row gap-1 items-center mb-2">
					<Ruler color="#82df9e" />
					<h2 class="scroll-m-20 mt-0 text-xl font-semibold tracking-tight w-fit">Skills</h2>
				</div>

				<p class="text">Svelte, Figma, HTML, CSS, JavaScript</p>
			</div>
			<div class="border-2 border-[#82df9e] rounded-lg p-4 bg-white w-full lg:w-fit">
				<div class="flex flex-row gap-1 items-center mb-2">
					<Users color="#82df9e" />
					<h2 class="scroll-m-20 mt-0 text-xl font-semibold tracking-tight w-fit">Team</h2>
				</div>

				<p class="text">Ethan Li (UX/UI), Tirsten Lisondra (UX/UI), Max Li (Project Supervisor)</p>
			</div>
			<div class="border-2 border-[#82df9e] rounded-lg p-4 bg-white w-full lg:w-fit">
				<div class="flex flex-row gap-1 items-center mb-2">
					<ExternalLink color="#82df9e" />
					<h2 class="scroll-m-20 mt-0 text-xl font-semibold tracking-tight w-fit">
						Link to Website
					</h2>
				</div>

				<a
					class="text-chart-2 hover:underline"
					target="_blank"
					href="https://greenbasilrestaurant.ca/">greenbasilrestaurant.ca</a
				>
			</div>
		</div>
		<img
			class="project-thumbnail mb-1 rounded-xl border-2 border-[#82df9e] w-full"
			src="/media/green-basil/gb-thumbnail.webp"
			alt="Green Basil Thai Restaurant Project Thumbnail"
		/>
	</section>
	<!-- <section class="pp-header mb-12 w-full flex flex-nowrap flex-col items-center">
		<div class="flex flex-col 2xl:flex-row xl:gap-8 justify-between w-full md:w-4/5">
			<div class="pp-details mb-4 w-full md:w-4/5">
				<h2 class="scroll-m-20 mt-0 text-2xl font-semibold tracking-tight">Details</h2>
				<ul class=" ms-6 list-disc [&>li]:mt-2">
					<li>Duration: March 2025 - May 2025</li>
					<li>
						See the finished project here: <a
							class="text-chart-1 hover:underline"
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
			<div class="pp-desc mb-4 w-full md:w-4/5">
				<h2 class="scroll-m-20 mt-0 text-2xl font-semibold tracking-tight">Overview</h2>
				<p class="text">
					Green Basil Thai Restaurant is located in Burnaby, BC, and has been a cornerstone of Thai
					cuisine since 2006. For this project, our team was tasked with redesigning and modernizing
					their website to appeal to a new generation of customers.
				</p>
			</div>
			<div class="pp-goals mb-4 w-full md:w-4/5">
				<h2 class="scroll-m-20 mt-0 text-2xl font-semibold tracking-tight">My Goals</h2>
				<p>
					In this project, my goal was to develop a website that was both functional and easy to
					use. Additionally, as we were not given a concrete deadline for the project, I took my
					time to learn as many new skills as possible, including how to use the UI framework known
					as Svelte.
				</p>
			</div>
		</div>
	</section> -->

	<section class="pp-process mb-24 w-full flex flex-nowrap flex-col items-center">
		<h2 class="scroll-m-20 mt-0 text-2xl font-semibold tracking-tight mb-6">Overview</h2>
		<div class="w-full md:w-4/5">
			<div class="flex flex-col 2xl:flex-row gap-1 justify-between">
				<h3 class="scroll-m-20 text-4xl font-semibold tracking-tight">
					Introduction to the Client
				</h3>
				<p>
					Green Basil Thai Restaurant is located in Burnaby, BC, and has been a cornerstone of Thai
					cuisine since 2006. For this project, our team was tasked with redesigning and modernizing
					their website to appeal to a new generation of customers.
				</p>
			</div>
		</div>
	</section>

	<section class="pp-process mb-24 w-full flex flex-nowrap flex-col items-center">
		<h2 class="scroll-m-20 mt-0 text-2xl font-semibold tracking-tight mb-6">The Problem</h2>
		<p class="scroll-m-20 text-4xl font-semibold tracking-tight text-center">
			How might we create a digital identity to appeal to a younger demographic of customers?
		</p>
	</section>
	<section class="pp-process mb-24 w-full flex flex-nowrap flex-col items-center">
		<h2 class="scroll-m-20 mt-0 text-2xl font-semibold tracking-tight mb-6">The Process</h2>
		<div class="w-full md:w-4/5 mb-12">
			<div class="flex flex-col 2xl:flex-row gap-1 justify-between">
				<h3 class="scroll-m-20 text-4xl font-semibold tracking-tight mb-2 md:mb-0">
					Stage 1: Making a Plan
				</h3>
				<div class="gap-4 flex flex-col">
					<p>
						I approached the planning stage with a learn-first mentality. This involved maintaining
						constant communication with the design team, and learning how to create all of the
						different pages and interactions using a Svelte, a new framework for me.
					</p>
					<p>
						As a result, I developed my collaboration and communication skills by offering my UX
						knowledge in team meetings to help the design team create user-friendly interactions.
					</p>
				</div>
			</div>
		</div>

		<div class="w-full md:w-4/5 mb-12">
			<div class="flex flex-col 2xl:flex-row gap-1 justify-between">
				<h3 class="scroll-m-20 text-4xl font-semibold tracking-tight mb-2 md:mb-0">
					Stage 2: Development
				</h3>
				<!-- <p>
					In the working process, I focused on constantly testing responsiveness, link validity, and
					interaction design, etc., to achieve the desired results. Additionally, I adopted a rigid
					schedule to keep myself on task and ensure that progress was always being made.
				</p> -->
				<div class="gap-4 flex flex-col">
					<p>
						Being the sole developer of the project, it was important for me to maintain constant
						communication with the devlopment team during the dev process to ensure all aspects of
						the site were executed accordingley. This also included regular check-ins with the
						client to keep them updated and get their approval on new changes.
					</p>
					<p>
						In the working process, I focused on constantly testing responsiveness, link validity,
						and interaction design, etc., to achieve the desired results. Additionally, I adopted a
						rigid schedule to keep myself on task and ensure that progress was always being made.
					</p>
				</div>
			</div>
			<video
				class="case-media my-6 rounded-xl border-2 border-[#82df9e] w-full"
				width="1458"
				height="830"
				autoplay
				loop
				muted
			>
				<source src="/media/green-basil/portfolio-gb-responsiveness.mp4" />
			</video>
		</div>

		<div class="w-full md:w-4/5 mb-12">
			<div class="flex flex-col 2xl:flex-row gap-1 justify-between">
				<h3 class="scroll-m-20 text-4xl font-semibold tracking-tight mb-2 md:mb-0">
					Stage 3: Reflection
				</h3>
				<div>
					<p class="mb-6">
						<span class="font-bold">The struggle: </span>As a first-time solo developer working with
						a lesser-known framework like Svelte, debugging was a tedious process. An instance of
						this was an issue with the snap-scrolling effect on certain pages, where the overflow
						margins would be incorrect, or other features would no longer function.
					</p>
					<p>
						<span class="font-bold">The solution: </span>While the fix ended up being a simple CSS
						error, an important thing that this taught me was to re-evaluate and come back to a
						problem with a different mindset. Instead of getting stuck on this one bug, I was able
						to be productive in other areas and develop separate skills, so that by the time this
						bug resurfaced to the top of my to-do list, I was ready to tackle it.
					</p>
				</div>
			</div>

			<video
				class="case-media my-6 rounded-xl border-2 border-[#82df9e] w-full"
				width="1904"
				height="944"
				autoplay
				loop
				muted
			>
				<source src="/media/green-basil/portfolio-gb-scrollsnap.mp4" />
			</video>
		</div>

		<div class="w-full md:w-4/5">
			<div class="flex flex-col 2xl:flex-row gap-1 justify-between">
				<h3 class="scroll-m-20 text-4xl font-semibold tracking-tight mb-2 md:mb-0">
					Stage 4: Going Forward
				</h3>
				<div>
					<h4 class="scroll-m-20 text-lg font-semibold tracking-tight">
						What I Would do Different
					</h4>
					<p class="mb-6">
						One of the main things I learned was the importance of web scaffolding. If I were to do
						this project again, rather than planning along the way, I would first collect all the
						data I need, organize it into JavaScript files that have the parameters of the data
						sorted into the groups needed, and then begin the HTML and CSS.
					</p>
					<h4 class="scroll-m-20 text-lg font-semibold tracking-tight">What I Learned</h4>
					<p>
						I gained many skills throughout this project, most significantly working within Svelte,
						a UI framework, for the first time. I learned about the importance of proper
						scaffolding, the length of the iterative process and debugging, and how to keep a
						consistent work schedule to keep a team motivated.
					</p>
				</div>
			</div>
		</div>
	</section>
	<!-- <section class="pp-process mb-12 w-full flex flex-nowrap flex-col items-center">
		<h2 class="scroll-m-20 mt-0 text-2xl font-semibold tracking-tight mb-4">Extra Content</h2>
		<div></div>
	</section> -->
</section>
