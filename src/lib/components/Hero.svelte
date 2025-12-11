<script lang="ts">
	// Customer logos
	const logos = [
		{ name: 'Cursor', width: 80 },
		{ name: 'Alan', width: 70 },
		{ name: 'Celonis', width: 90 },
		{ name: 'Trimble', width: 80 },
		{ name: 'Nordic Semi', width: 100 },
		{ name: 'SmithRx', width: 80 },
		{ name: 'Jump Trading', width: 100 },
		{ name: 'Archer', width: 70 },
		{ name: 'XGBoost', width: 80 },
		{ name: 'Collective', width: 90 }
	];
</script>

<section class="relative pt-32 pb-16 px-6 md:px-12 max-w-7xl mx-auto min-h-screen flex flex-col justify-between">
	<div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
		<div class="z-10">
			<h1 class="text-6xl md:text-7xl lg:text-8xl font-display font-medium text-gray-900 leading-[0.9] tracking-tight mb-8">
				10x cheaper<br>
				<span class="text-brand-green">GitHub Actions</span>
			</h1>
			
			<div class="relative w-12 h-12 mb-8">
				<!-- Speed icon -->
				<svg viewBox="0 0 24 24" fill="none" class="w-10 h-10 text-brand-green absolute top-0 left-0">
					<path d="M13 2L3 14h8l-1 8 10-12h-8l1-8z" fill="currentColor" opacity="0.8"/>
				</svg>
			</div>

			<div class="space-y-6 max-w-lg">
				<p class="font-mono text-sm text-gray-700 uppercase tracking-wider leading-relaxed">
					SELF-HOSTED AWS EC2 RUNNERS<br>
					WITH S3 CACHING FOR BLAZING FAST<br>
					CI/CD AT A FRACTION OF THE COST
				</p>

				<div class="flex flex-col items-start gap-3">
					<a href="https://runs-on.com/pricing" class="bg-black text-white px-6 py-3 rounded text-sm font-medium hover:bg-gray-800 transition-colors flex items-center gap-2">
						Start Free Trial
						<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14"/><path d="m12 5 7 7-7 7"/></svg>
					</a>
					<p class="text-[10px] text-gray-500 font-mono uppercase tracking-wide">
						15-day free trial • Setup in 10 minutes
					</p>
				</div>
			</div>
		</div>

		<div class="relative h-[400px] lg:h-[600px] w-full flex items-center justify-center">
			<!-- AWS Infrastructure Illustration -->
			<div class="absolute inset-0 flex items-center justify-center">
				<div class="relative w-full h-full max-w-md">
					<!-- Simple AWS architecture diagram -->
					<svg viewBox="0 0 400 400" class="w-full h-full">
						<!-- GitHub Actions -->
						<g transform="translate(200, 50)">
							<rect x="-40" y="-20" width="80" height="40" rx="4" fill="black" opacity="0.9"/>
							<text x="0" y="5" text-anchor="middle" fill="white" font-size="12" font-family="monospace">GitHub</text>
						</g>
						
						<!-- Arrow down -->
						<path d="M200,90 L200,140" stroke="oklch(0.596 0.145 163.225)" stroke-width="2" marker-end="url(#arrowhead)"/>
						
						<!-- RunsOn Controller -->
						<g transform="translate(200, 160)">
							<rect x="-50" y="-25" width="100" height="50" rx="4" fill="oklch(0.596 0.145 163.225)" opacity="0.2" stroke="oklch(0.596 0.145 163.225)" stroke-width="2"/>
							<text x="0" y="5" text-anchor="middle" fill="black" font-size="12" font-family="monospace" font-weight="bold">RunsOn</text>
						</g>
						
						<!-- Arrows to EC2 instances -->
						<path d="M200,185 L100,240" stroke="oklch(0.596 0.145 163.225)" stroke-width="2" marker-end="url(#arrowhead)"/>
						<path d="M200,185 L200,240" stroke="oklch(0.596 0.145 163.225)" stroke-width="2" marker-end="url(#arrowhead)"/>
						<path d="M200,185 L300,240" stroke="oklch(0.596 0.145 163.225)" stroke-width="2" marker-end="url(#arrowhead)"/>
						
						<!-- EC2 Instances -->
						<g transform="translate(100, 270)">
							<rect x="-35" y="-20" width="70" height="40" rx="4" fill="white" stroke="gray" stroke-width="1"/>
							<text x="0" y="5" text-anchor="middle" fill="gray" font-size="10" font-family="monospace">EC2</text>
						</g>
						<g transform="translate(200, 270)">
							<rect x="-35" y="-20" width="70" height="40" rx="4" fill="white" stroke="gray" stroke-width="1"/>
							<text x="0" y="5" text-anchor="middle" fill="gray" font-size="10" font-family="monospace">EC2</text>
						</g>
						<g transform="translate(300, 270)">
							<rect x="-35" y="-20" width="70" height="40" rx="4" fill="white" stroke="gray" stroke-width="1"/>
							<text x="0" y="5" text-anchor="middle" fill="gray" font-size="10" font-family="monospace">EC2</text>
						</g>
						
						<!-- S3 Cache -->
						<g transform="translate(200, 350)">
							<rect x="-45" y="-20" width="90" height="40" rx="4" fill="white" stroke="oklch(0.596 0.145 163.225)" stroke-width="2" stroke-dasharray="4,4"/>
							<text x="0" y="5" text-anchor="middle" fill="oklch(0.596 0.145 163.225)" font-size="11" font-family="monospace" font-weight="bold">S3 Cache</text>
						</g>
						
						<!-- Arrow markers -->
						<defs>
							<marker id="arrowhead" markerWidth="10" markerHeight="10" refX="9" refY="3" orient="auto">
								<polygon points="0 0, 10 3, 0 6" fill="oklch(0.596 0.145 163.225)" />
							</marker>
						</defs>
					</svg>
				</div>
			</div>
		</div>
	</div>

	<div class="mt-20 border-t border-gray-300 pt-8">
		<div class="flex items-center gap-2 text-[10px] font-mono uppercase tracking-wider text-gray-600 mb-6">
			500+ ENGINEERING TEAMS • PROCESSING 500K+ JOBS DAILY
		</div>
		
		<div class="grid grid-cols-2 md:grid-cols-5 gap-8 opacity-60 grayscale">
			{#each logos as logo}
				<div class="h-8 flex items-center justify-center border border-gray-300/50 rounded bg-gray-100/50">
					<span class="text-xs font-bold text-gray-500">{logo.name}</span>
				</div>
			{/each}
		</div>
	</div>
</section>
