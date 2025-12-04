<script lang="ts">
	import CalendarIcon from '@lucide/svelte/icons/calendar';
	import HouseIcon from '@lucide/svelte/icons/house';
	import InboxIcon from '@lucide/svelte/icons/inbox';
	import SearchIcon from '@lucide/svelte/icons/search';
	import SettingsIcon from '@lucide/svelte/icons/settings';
	import * as Sidebar from '$lib/components/ui/sidebar/index.js';
	import * as DropdownMenu from '$lib/components/ui/dropdown-menu/index.js';
	import { Badge } from '$lib/components/ui/badge/index.js';

	// Menu items.
	const items = [
		{
			title: 'Home',
			url: '/',
			icon: HouseIcon
		}
		// {
		// 	title: 'About',
		// 	url: '#'
		// 	//    icon: InboxIcon,
		// }
		//   {
		//    title: "Calendar",
		//    url: "#",
		//    icon: CalendarIcon,
		//   },
		//   {
		//    title: "Search",
		//    url: "#",
		//    icon: SearchIcon,
		//   },
		//   {
		//    title: "Settings",
		//    url: "#",
		//    icon: SettingsIcon,
		//   },
	];

	const project_items = [
		{
			title: 'Green Basil Website',
			url: '/projects/green-basil',
			badge: 'Lead Front-End'
			//    icon: HouseIcon,
		},
		{
			title: '(WIP) Industry Media Group',
			url: '/projects/industry-media',
			badge: 'Junior Front-End'
			//    icon: HouseIcon,
		},
		{
			title: '(WIP) Mosaic: Event App',
			url: '/projects/mosaic',
			badge: 'UI/UX Design & Motion Graphics'
			//    icon: HouseIcon,
		},
		{
			title: '(WIP) Bankment: A Stellar New Year',
			url: '/projects/bankment-stellar',
			badge: 'Product Design'
			//    icon: HouseIcon,
		}
	];

	const footer_items = [
		{
			title: 'LinkedIn',
			url: 'https://www.linkedin.com/feed/'
			//    icon: HouseIcon,
		},
		{
			title: 'Github',
			url: 'https://github.com/nathan-gg'
			//    icon: HouseIcon,
		},
		{
			title: 'Email',
			url: 'mailto:nsgebreab@gmail.com'
			//    icon: HouseIcon,
		},
		{
			title: 'Resume',
			url: '/documents/NathanGebreab_Resume.pdf'
			//    icon: HouseIcon,
		}
	];
</script>

<Sidebar.Root>
	<Sidebar.Content>
		<Sidebar.Group>
			<Sidebar.GroupLabel>Nathan Gebreab</Sidebar.GroupLabel>
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
										<!-- <item.icon /> -->
										<span>{item.title}</span>
									</a>
									<Badge variant="outline" class="ml-2 mb-1 text-muted-foreground"
										>{item.badge}</Badge
									>
								{/snippet}
							</Sidebar.MenuButton>
						</Sidebar.MenuItem>
					{/each}
				</Sidebar.Menu>
			</Sidebar.GroupContent>
		</Sidebar.Group>
	</Sidebar.Content>
	<Sidebar.Footer>
		<Sidebar.Group>
			<Sidebar.GroupLabel>See More</Sidebar.GroupLabel>
			<Sidebar.GroupContent>
				<Sidebar.Menu>
					{#each footer_items as item (item.title)}
						<Sidebar.MenuItem>
							<Sidebar.MenuButton>
								{#snippet child({ props })}
									<a href={item.url} target="_blank" {...props}>
										<!-- <item.icon /> -->
										<span>{item.title}</span>
									</a>
								{/snippet}
							</Sidebar.MenuButton>
						</Sidebar.MenuItem>
					{/each}
				</Sidebar.Menu>
			</Sidebar.GroupContent>
		</Sidebar.Group>
	</Sidebar.Footer>
</Sidebar.Root>
