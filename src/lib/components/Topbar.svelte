<script lang="ts">
	import { onMount } from 'svelte';

	export let showOnScroll: boolean = true; // Default to true, so it shows on scroll

	let isVisible = false;

	// Function to detect scroll position and update the visibility of the top bar
	const handleScroll = () => {
		if (window.scrollY > 50 && showOnScroll) {
			isVisible = true;
		} else {
			isVisible = false;
		}
	};

	// Add the scroll event listener when the component is mounted
	onMount(() => {
		if (showOnScroll) {
			window.addEventListener('scroll', handleScroll);
		}

		// Clean up the event listener when the component is destroyed
		return () => {
			window.removeEventListener('scroll', handleScroll);
		};
	});
</script>

<!-- Topbar -->
<div
	class="fixed top-0 right-0 left-0 z-50 h-16 transform bg-gray-800 px-6 py-4 text-center text-white transition-transform"
	class:translate-y-[-100%]={!isVisible}
>
	<h1>My Top Bar</h1>
</div>
