<script lang="ts">
	import { HeroParallax } from '$lib/components/ui/HeroParallax/index.js';
	import Topbar from '$lib/components/Topbar.svelte';
	import Icon from '@iconify/svelte';

	const products = [
		{
			title: 'Payment Summary',
			link: '',
			thumbnail: '/ui_designs/Summary.png'
		},
		{
			title: 'Career Fair',
			link: '',
			thumbnail: '/ui_designs/CareerFair.png'
		},
		{
			title: 'Landing',
			link: '',
			thumbnail: '/ui_designs/Landing.png'
		},

		{
			title: 'CGPT',
			link: '',
			thumbnail: '/ui_designs/CGPT.png'
		},
		{
			title: 'Copilot AI',
			link: '',
			thumbnail: '/ui_designs/Copilot.png'
		},
		{
			title: 'Core Services',
			link: '',
			thumbnail: '/ui_designs/CoreServices.png'
		},

		{
			title: 'Facility View',
			link: '',
			thumbnail: '/ui_designs/FacilityView.png'
		},

		{
			title: 'Giftcard',
			link: '',
			thumbnail: '/ui_designs/Giftcard.png'
		},

		{
			title: 'POS Cards',
			link: '',
			thumbnail: '/ui_designs/POS_Cards.png'
		},
		{
			title: 'Sign In',
			link: '',
			thumbnail: '/ui_designs/SignIn.png'
		},
		{
			title: 'Electric Carbon Emission',
			link: '',
			thumbnail: '/ui_designs/ElectricEmission.png'
		},
		{
			title: 'Giftcard Email',
			link: '',
			thumbnail: '/ui_designs/Giftcard_Email.png'
		},
		{
			title: 'Groceries',
			link: '',
			thumbnail: '/ui_designs/Groceries.png'
		},
		{
			title: 'Grocer Chat',
			link: '',
			thumbnail: '/ui_designs/Grocer_Chat.png'
		},
		{
			title: 'Petrol Carbon Emission',
			link: '',
			thumbnail: '/ui_designs/PetrolEmission.png'
		}
	];

	const projects = [
		{
			id: 'cgpt-website',
			title: 'Company Website: Carbon GPT',
			description:
				'Official website for Carbon GPT, showcasing the product and its features. The design focuses on user experience and modern aesthetics, with a clean layout and intuitive navigation.',
			image: '/previews/cgpt-web.png',
			link: 'https://www.carbongpt.ai/home',
			skills: ['Web Design', 'Product', 'Modern Design', 'SvelteKit']
		},
		{
			id: 'food-app',
			title: 'Mobile App: Food Ordering & Loyalty Points',
			description:
				'A mobile app prototype with interactive components for ordering food and managing loyalty points, designed with user experience as the primary focus.',
			image: '/previews/loyalty-app.png',
			link: 'https://www.figma.com/proto/edYA8UgECvdXwsCYJj7BQW/Loyalty-Program-Mobile-App?page-id=193%3A1273&node-id=193-1455&starting-point-node-id=193%3A1455&t=jat5gO37feRiXLMS-1',
			skills: ['Mobile Design', 'Prototyping', 'Interaction Design', 'Figma']
		},
		{
			id: 'pdf-sample',
			title: 'PDF Export Mockup',
			description:
				'A mockup on the pdf view of a sustainability report. This report is a sample of a project I worked on, showcasing the design and layout of the report.',
			image: '/previews/pdf.png',
			link: 'https://www.figma.com/design/ZYlIHxDfltDSfHPZ6eJgoU/AI-SR-Sample-Full-Report?node-id=0-1',
			skills: ['PDF Report', 'Prototyping', 'Figma']
		},
		{
			id: 'capstone',
			title: 'Capstone Project: Mobile Grocery Application',
			description:
				'Final Year Project UI/UX Planning and Prototype. A grocery mobile app with chatbot that helps users filter through items, search for items, compare items, and add items to the cart through text.',
			image: '/previews/fyp.png',
			link: 'https://www.figma.com/design/hq6yaQYTRuRLJ4IEdYMXhq/Capstone-Project-2024?node-id=134-2',
			skills: ['Mobile Design', 'UI/UX', 'Chatbot Interface', 'Figma']
		},
		{
			id: 'web-redesign',
			title: 'UI/UX Exercise: Government Job Portal Redesign',
			description:
				'An exercise on redesigning a government-developed job portal with Wireframe and Prototype, focusing on improved user experience and modern design principles.',
			image: '/previews/MFJ-redesign.png',
			link: 'https://www.figma.com/design/2kfzfdPaUidQmFdt0C9O6y/UI-UX---Proposed-Web-Redesign?node-id=1-2',
			skills: ['Web Design', 'Wireframing', 'UI/UX', 'Figma']
		},
		{
			id: 'in-development',
			title: 'UI/UX on In-Development Projects',
			description:
				'Redesigning and creating new UI for pages initially built as PoC. Components were reevaluated for UX with many aspects changed and proposed for two products and graphical design assets for the company website.',
			image: '/previews/pos.png',
			link: 'https://www.figma.com/design/aknxaws6ALJU9U0qjT7guF/UI%2FUX-Design?node-id=0-1&t=aC08Mp9JqxfhstB1-1',
			skills: ['Web Design', 'UI/UX', 'Component Design', 'Figma']
		}
	];
</script>

<main class="flex w-full flex-col">
	<!-- <Topbar /> -->
	<HeroParallax {products} />

	<div class="flex flex-col space-y-32 px-10 py-10">
		<section class="my-20">
			<div class="overflow-hidden rounded-xl bg-white shadow-xl dark:bg-gray-800">
				<div class="p-8 md:p-12">
					<h2 class="dark:prose-invert mb-6 text-3xl font-bold md:text-4xl">My Resume</h2>
					<div class="flex flex-col items-center gap-8 md:flex-row">
						<div class="relative w-full md:w-2/3">
							<div
								class="relative aspect-[8.5/11] overflow-hidden rounded-lg border border-gray-200 shadow-lg dark:border-gray-700"
							>
								<img
									src={'/previews/resume.png'}
									alt="Resume Preview"
									width="800"
									height="600"
									class="object-fit h-full w-auto transition-transform duration-500 group-hover:scale-105"
								/>
							</div>
						</div>
						<div class="w-full space-y-6 md:w-1/3">
							<div class="prose dark:prose-invert">
								<h3 class="text-xl font-semibold">Download My Resume</h3>
								<p>
									View my qualifications, experience, and skills in detail. Download a copy of my
									resume for your reference.
								</p>
							</div>
							<a
								href="/files/Resume.pdf"
								download
								class="inline-flex items-center justify-center rounded-md bg-purple-600 px-4 py-2 text-sm font-medium text-white shadow-sm hover:bg-purple-700 focus:ring-2 focus:ring-purple-500 focus:ring-offset-2 focus:outline-none"
							>
								<Icon icon="lucide:download" class="mr-2 h-5 w-5" />
								Download PDF Resume
							</a>
							<div class="pt-4 text-sm text-gray-500 dark:text-gray-400">
								<p>Last updated: May 2024</p>
							</div>
						</div>
					</div>
				</div>
			</div>
		</section>

		<header class="mb-16 flex h-auto flex-col text-center">
			<h1
				class="h mb-4 bg-gradient-to-r from-purple-600 to-pink-600 bg-clip-text text-3xl font-bold text-transparent md:text-4xl"
			>
				UI/UX Design Projects
			</h1>
			<p class="mx-auto max-w-2xl text-lg text-gray-600 dark:text-gray-300">
				A showcase of my design work across mobile applications and web interfaces, demonstrating my
				approach to creating intuitive and engaging user experiences.
			</p>
		</header>

		{#each projects as project, index}
			<section
				class="flex flex-col {index % 2 === 0
					? 'md:flex-row'
					: 'md:flex-row-reverse'} items-center gap-8 md:gap-12"
			>
				<div class="group relative w-full md:w-1/2">
					<div class="relative overflow-hidden rounded-xl shadow-xl">
						<div
							class="absolute inset-0 z-10 bg-gradient-to-tr from-purple-500/20 to-pink-500/20 opacity-0 transition-opacity duration-300 group-hover:opacity-100"
						></div>
						<img
							src={project.image || '/placeholder.svg'}
							alt={project.title}
							width="800"
							height="600"
							class="h-auto w-full object-cover transition-transform duration-500 group-hover:scale-105"
						/>
					</div>
					<div
						class="absolute -right-4 -bottom-4 transform rounded-lg bg-white p-3 shadow-lg transition-transform duration-300 group-hover:translate-x-2 group-hover:translate-y-2 dark:bg-gray-800"
					>
						<a
							href={project.link}
							target="_blank"
							rel="noopener noreferrer"
							class="flex items-center gap-1 text-sm font-medium text-purple-600 dark:text-purple-400"
						>
							<span>View in Figma</span>
							<Icon icon="lucide:external-link" />
						</a>
					</div>
				</div>

				<div class="w-full space-y-4 md:w-1/2">
					<h2 class="text-2xl font-bold md:text-3xl">{project.title}</h2>
					<p class="text-gray-600 dark:text-gray-300">{project.description}</p>

					<div class="flex flex-wrap gap-2 pt-2">
						{#each project.skills as skill}
							<span
								class="rounded-full bg-purple-100 px-3 py-1 text-sm text-purple-700 dark:bg-purple-700 dark:text-purple-300"
							>
								{skill}
							</span>
						{/each}
					</div>

					<a
						href={project.link}
						target="_blank"
						rel="noopener noreferrer"
						class="group mt-4 inline-flex items-center justify-center rounded-md bg-purple-600 px-4 py-2 text-sm font-medium text-white shadow-sm hover:bg-purple-700 focus:ring-2 focus:ring-purple-500 focus:ring-offset-2 focus:outline-none"
					>
						Explore Project
						<Icon
							icon="lucide:arrow-right"
							class="ml-2 h-4 w-4 transition-transform group-hover:translate-x-1"
						/>
					</a>
				</div>
			</section>
		{/each}
	</div>
</main>
