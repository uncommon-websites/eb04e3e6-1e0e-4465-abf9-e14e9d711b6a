<script lang="ts">
	import { onMount } from 'svelte';
	
	let isScrolled = false;

	onMount(() => {
		const handleScroll = () => {
			isScrolled = window.scrollY > 20;
		};
		window.addEventListener('scroll', handleScroll);
		return () => window.removeEventListener('scroll', handleScroll);
	});
</script>

<header class="fixed top-0 left-0 right-0 z-50 transition-all duration-300 px-6 py-4 flex items-center justify-between {isScrolled ? 'bg-[#EAEAE8]/90 backdrop-blur-md border-b border-gray-200' : 'bg-transparent'}">
	<div class="flex items-center gap-8">
		<a href="/" class="flex items-center gap-2 text-brand-dark font-medium text-xl tracking-tight">
			<svg width="24" height="30" viewBox="0 0 90 115" fill="none" xmlns="http://www.w3.org/2000/svg">
				<path fill-rule="evenodd" clip-rule="evenodd" d="M31.8701 9.95388L15.3109 19.4791L31.8819 29.0064L48.446 19.4812L31.8701 9.95388ZM53.2588 27.7795L36.6927 37.3058L36.6911 56.3603L53.2588 46.8319V27.7795ZM58.0696 55.1313L41.5014 64.66L58.072 74.187L74.6383 64.6605L58.0696 55.1313ZM79.4486 72.9601L62.883 82.4862V101.538L79.4486 92.0122V72.9601ZM53.2614 101.539V82.4864L36.6903 72.9591V92.012L53.2614 101.539ZM27.0694 56.3613L10.5003 46.8319V27.7788L27.0711 37.3058L27.0694 56.3613ZM27.0687 67.4269L4.48643 54.4394C2.25391 53.1554 0.878662 50.7828 0.878662 48.215V19.4801C0.878662 17.7684 1.79538 16.1867 3.28356 15.3307L28.2608 0.963381C30.4933 -0.320696 33.2439 -0.321154 35.4766 0.962171L60.474 15.3299C61.963 16.1857 62.8804 17.7679 62.8804 19.4801V46.8319L86.665 60.5111C88.1535 61.3671 89.0702 62.9489 89.0702 64.6607V93.3956C89.0702 95.9635 87.6948 98.3361 85.4621 99.62L60.4776 113.988C58.9894 114.843 57.1558 114.843 55.6673 113.988L30.6773 99.6202C28.4444 98.3365 27.0687 95.9635 27.0687 93.3954V67.4269Z" fill="black"/>
			</svg>
			RunsOn
		</a>
		
		<nav class="hidden md:flex items-center gap-6 text-sm font-medium text-gray-600">
			<a href="https://runs-on.com/pricing" class="hover:text-gray-900 transition-colors">Pricing</a>
			<a href="https://runs-on.com/guides" class="hover:text-gray-900 transition-colors">Guides</a>
			<a href="https://runs-on.com/docs" class="hover:text-gray-900 transition-colors">Docs</a>
			<a href="https://github.com/runs-on/runs-on" class="hover:text-gray-900 transition-colors flex items-center gap-1">
				GitHub
				<svg xmlns="http://www.w3.org/2000/svg" width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M7 7h10v10"/><path d="M7 17 17 7"/></svg>
			</a>
		</nav>
	</div>

	<div class="flex items-center gap-4">
		<a href="https://runs-on.com/docs" class="text-sm font-medium text-gray-700 hover:text-gray-900 transition-colors">Documentation</a>
		<a href="https://runs-on.com/pricing" class="text-sm font-medium text-white bg-black px-4 py-2 rounded hover:bg-gray-800 transition-colors">Start Free Trial</a>
	</div>
</header>
