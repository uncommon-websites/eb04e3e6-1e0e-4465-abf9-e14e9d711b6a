<script lang="ts">
	import { slide } from 'svelte/transition';

	const faqs = [
		{
			question: "How does RunsOn pricing work?",
			answer: "RunsOn has three tiers: Demo (free 15-day trial), Commercial (€300/year), and Sponsorship (€1,500/year with source code access). You pay AWS costs directly at actual rates - no markup."
		},
		{
			question: "How long does setup take?",
			answer: "Setup takes about 10 minutes. Deploy the CloudFormation stack, add your license key to GitHub secrets, and update your workflow YAML. That's it."
		},
		{
			question: "Does RunsOn work with private repositories?",
			answer: "Yes, RunsOn works with both public and private repositories. It runs entirely in your AWS account with no third-party access."
		},
		{
			question: "What's the difference between RunsOn and Actions Runner Controller?",
			answer: "RunsOn is simpler - no Kubernetes required. It uses native AWS services (EC2, S3, Lambda) and includes features like S3 caching and automatic cost attribution that ARC doesn't have."
		},
		{
			question: "Can I use RunsOn with GitHub Enterprise?",
			answer: "Yes, RunsOn works with GitHub.com, GitHub Enterprise Cloud, and GitHub Enterprise Server."
		},
		{
			question: "What AWS regions are supported?",
			answer: "RunsOn supports all major AWS regions. You choose the region during CloudFormation deployment."
		},
		{
			question: "Is there support for non-profit organizations?",
			answer: "Yes, RunsOn offers free non-commercial licenses for non-profit organizations."
		}
	];

	let openIndex: number | null = null;

	function toggle(index: number) {
		openIndex = openIndex === index ? null : index;
	}
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto border-t border-gray-200">
	<div class="grid grid-cols-1 lg:grid-cols-3 gap-12">
		<div>
			<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
				[ FAQ ]
			</span>
			<h2 class="font-display text-4xl md:text-5xl font-medium tracking-tight text-gray-900 mb-6">
				Frequently Asked Questions
			</h2>
			<p class="font-mono text-sm text-gray-600 mb-8">
				Your question not answered here?
			</p>
			<button class="bg-brand-green text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-brand-green-hover transition-colors flex items-center gap-2 font-mono uppercase tracking-wide text-xs">
				<svg xmlns="http://www.w3.org/2000/svg" width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"/></svg>
				Contact Us
			</button>
		</div>

		<div class="lg:col-span-2 space-y-4">
			{#each faqs as faq, i}
				<div class="border-b border-gray-200 pb-4">
					<button class="w-full flex items-center justify-between text-left py-2 group" on:click={() => toggle(i)}>
						<span class="font-mono text-sm font-medium text-gray-800 group-hover:text-brand-green transition-colors pr-8">{faq.question}</span>
						<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-gray-400 transition-transform duration-300 {openIndex === i ? 'rotate-180' : ''}"><path d="m6 9 6 6 6-6"/></svg>
					</button>
					{#if openIndex === i}
						<div transition:slide={{ duration: 300 }} class="overflow-hidden">
							<p class="pt-2 pb-4 text-sm text-gray-600 leading-relaxed max-w-2xl font-mono">
								{faq.answer}
							</p>
						</div>
					{/if}
				</div>
			{/each}
		</div>
	</div>
</section>
