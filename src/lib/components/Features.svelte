<script lang="ts">
	import FeatureCard from './FeatureCard.svelte';
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto relative" id="features">
    <!-- Background Grid Pattern -->
    <div class="absolute inset-0 z-0 opacity-30 pointer-events-none" 
        style="background-image: linear-gradient(#ccc 1px, transparent 1px), linear-gradient(90deg, #ccc 1px, transparent 1px); background-size: 40px 40px; mask-image: linear-gradient(to bottom, transparent, black 10%, black 90%, transparent);">
    </div>

	<div class="flex flex-col md:flex-row justify-between items-start md:items-end mb-16 gap-6 relative z-10">
		<div>
			<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
				[ WHY RUNSON ]
			</span>
			<h2 class="font-display text-4xl md:text-5xl lg:text-6xl font-medium tracking-tight text-gray-900 mb-4">
				Fast. Simple. Affordable.
			</h2>
			<p class="font-mono text-sm text-gray-600 max-w-lg">
				Self-hosted GitHub Actions runners on AWS EC2 with S3 caching. 10x cheaper than GitHub-hosted runners.
			</p>
		</div>
		
		<a href="https://runs-on.com/docs" class="bg-black text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-gray-800 transition-colors flex items-center gap-2 font-mono uppercase tracking-wide text-xs">
			Read the docs ->
		</a>
	</div>

	<div class="grid grid-cols-1 md:grid-cols-2 gap-6">
		<FeatureCard 
			subtitle="[ 10X COST SAVINGS ]"
			title="Pay only for<br>what you use"
			description="Run on AWS EC2 at actual cost. No markup, no hidden fees. Transparent AWS billing."
			tagColor="bg-brand-green"
			tagIcon="arrow"
            imageSrc="/generated/image-devops-engineer-looking-at-computer-scre-1765486797699-0.webp"
		/>
		
		<FeatureCard 
			subtitle="[ MAGIC CACHE ]"
			title="5x faster builds<br>with S3 caching"
			description="Transparent S3-based caching that's 5x faster than GitHub's cache. Plus EBS snapshot caching for Docker."
			tagColor="bg-accent-orange"
			tagIcon="plus"
            imageSrc="/generated/image-abstract-visualization-of-fast-data-tran-1765486811754-5.webp"
		/>
		
		<FeatureCard 
			subtitle="[ SIMPLE SETUP ]"
			title="10 minutes from<br>zero to running"
			description="CloudFormation stack deploys everything. Just add 'runs-on' to your workflow YAML. That's it."
			tagColor="bg-accent-pink"
			tagIcon="arrow"
            imageSrc="/generated/image-close-up-of-hands-typing-on-laptop-with--1765486809082-4.webp"
		/>
		
		<FeatureCard 
			subtitle="[ FULLY SELF-HOSTED ]"
			title="Your AWS account,<br>your control"
			description="Runs entirely in your AWS account. No third-party access. Full code transparency."
			tagColor="bg-accent-yellow"
			tagIcon="plus"
            imageSrc="/generated/image-server-racks-in-a-modern-data-center-wit-1765486801041-1.webp"
		/>
	</div>
</section>
