<script lang="ts">
	import CalendarIcon from '@lucide/svelte/icons/calendar';
	import HouseIcon from '@lucide/svelte/icons/house';
	import Folder from '@lucide/svelte/icons/folder';
	import Linkedin from '@lucide/svelte/icons/linkedin';
	import Github from '@lucide/svelte/icons/github';
	import Mail from '@lucide/svelte/icons/mail';
	import FileText from '@lucide/svelte/icons/file-text';
	import Utensils from '@lucide/svelte/icons/utensils';

	import * as Sidebar from '$lib/components/ui/sidebar/index.js';
	import { Badge } from '$lib/components/ui/badge/index.js';

	// Menu items.
	const items = [
		{
			title: 'Home',
			url: '/',
			icon: HouseIcon
		}
	];

	const project_items = [
		{
			title: 'Green Basil Website',
			url: '/projects/green-basil',
			badge: 'Lead Front-End',
			icon: Utensils
		}
	];

	const footer_items = [
		{
			title: 'LinkedIn',
			url: 'https://www.linkedin.com/in/nathangebreab/',
			icon: Linkedin
		},
		{
			title: 'Github',
			url: 'https://github.com/nathan-gg',
			icon: Github
		},
		{
			title: 'Email',
			url: 'mailto:nsgebreab@gmail.com',
			icon: Mail
		},
		{
			title: 'Resume',
			url: '/documents/NathanGebreab_Resume.pdf',
			icon: FileText
		}
	];
</script>

<Sidebar.Sidebar collapsible="icon">
	<!-- <Sidebar.Header>
		<Sidebar.Menu>
			<Sidebar.MenuItem>
				<Sidebar.MenuButton size="lg">
					{#snippet child({ props })}
						<div {...props} class="flex flex-col gap-0.5 leading-none">
							<span class="font-semibold">Nathan Gebreab</span>
							<span class="text-xs">Portfolio</span>
						</div>
					{/snippet}
				</Sidebar.MenuButton>
			</Sidebar.MenuItem>
		</Sidebar.Menu>
	</Sidebar.Header> -->

	<Sidebar.Content>
		<Sidebar.Group>
			<Sidebar.GroupLabel>Navigation</Sidebar.GroupLabel>
			<Sidebar.GroupContent>
				<Sidebar.Menu>
					{#each items as item (item.title)}
						<Sidebar.MenuItem>
							<Sidebar.MenuButton>
								{#snippet child({ props })}
									<a href={item.url} {...props}>
										<item.icon />
										<span>{item.title}</span>
									</a>
								{/snippet}
							</Sidebar.MenuButton>
						</Sidebar.MenuItem>
					{/each}
				</Sidebar.Menu>
			</Sidebar.GroupContent>
		</Sidebar.Group>

		<Sidebar.Group>
			<Sidebar.GroupLabel>Projects</Sidebar.GroupLabel>
			<Sidebar.GroupContent>
				<Sidebar.Menu>
					{#each project_items as item (item.title)}
						<Sidebar.MenuItem>
							<Sidebar.MenuButton>
								{#snippet child({ props })}
									<a href={item.url} {...props}>
										<item.icon color="#40af46" />
										<span>{item.title}</span>
									</a>
									<!-- <Badge variant="outline" class="ml-8 mb-1 text-muted-foreground"
										>{item.badge}</Badge
									> -->
								{/snippet}
							</Sidebar.MenuButton>
						</Sidebar.MenuItem>
					{/each}
				</Sidebar.Menu>
			</Sidebar.GroupContent>
		</Sidebar.Group>
	</Sidebar.Content>

	<Sidebar.Footer>
		<Sidebar.Menu>
			{#each footer_items as item (item.title)}
				<Sidebar.MenuItem>
					<Sidebar.MenuButton size="sm">
						{#snippet child({ props })}
							<a href={item.url} target="_blank" {...props}>
								<item.icon />
								<span>{item.title}</span>
							</a>
						{/snippet}
					</Sidebar.MenuButton>
				</Sidebar.MenuItem>
			{/each}
		</Sidebar.Menu>
	</Sidebar.Footer>
</Sidebar.Sidebar>

<style>
	:global([data-slot='sidebar-inner']) {
		border-top-right-radius: 1rem;
		border-bottom-right-radius: 1rem;
	}
</style>
