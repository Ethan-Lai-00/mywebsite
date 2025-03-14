<script lang="ts">
	import { HeroParallax } from '$lib/components/ui/HeroParallax/index.js';
	import Topbar from '$lib/components/Topbar.svelte';

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
</script>

<main class="flex w-full flex-col">
	<Topbar />
	<HeroParallax {products} />

	<!-- Additional Section 1 -->
	<section class=" bg-gray-100 py-16">
		<div class="mx-auto max-w-7xl px-4">
			<h2 class="text-3xl font-bold">Our Services</h2>
			<p class="mt-4 text-xl">We provide a range of services tailored to your needs.</p>
			<div class="mt-8 grid grid-cols-1 gap-8 md:grid-cols-2 lg:grid-cols-3">
				<div class="rounded-lg bg-white p-6 shadow-lg">
					<h3 class="text-xl font-semibold">Web Development</h3>
					<p class="mt-4">We create beautiful, responsive websites to help businesses grow.</p>
				</div>
				<div class="rounded-lg bg-white p-6 shadow-lg">
					<h3 class="text-xl font-semibold">App Development</h3>
					<p class="mt-4">Our apps deliver seamless experiences for users across devices.</p>
				</div>
				<div class="rounded-lg bg-white p-6 shadow-lg">
					<h3 class="text-xl font-semibold">UI/UX Design</h3>
					<p class="mt-4">We design user-centric interfaces that engage and delight users.</p>
				</div>
			</div>
		</div>
	</section>
</main>
