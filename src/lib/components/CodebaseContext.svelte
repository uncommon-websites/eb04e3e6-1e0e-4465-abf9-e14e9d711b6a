<section class="bg-gray-50 py-24 px-6 md:px-12 relative overflow-hidden">
	<div class="max-w-7xl mx-auto grid grid-cols-1 lg:grid-cols-2 gap-12 items-center relative z-10">
		<div>
			<span class="font-mono text-[10px] text-gray-600 uppercase tracking-widest mb-4 block">
				[ AWS-NATIVE ARCHITECTURE ]
			</span>
			<h2 class="font-display text-4xl md:text-5xl lg:text-6xl font-medium tracking-tight text-gray-900 mb-6 leading-[0.95]">
				Built for<br>AWS Scale
			</h2>
			<p class="font-mono text-sm text-gray-700 max-w-md mb-8 leading-relaxed">
				RunsOn uses AWS-native services for maximum performance. EC2 for compute, S3 for caching, CloudFormation for deployment. Handles 500k+ jobs per day in production.
			</p>
			
			<a href="https://runs-on.com/docs/architecture" class="bg-black text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-gray-800 transition-colors flex items-center gap-2 font-mono uppercase tracking-wide text-xs w-fit">
				View architecture ->
			</a>
		</div>

		<div class="relative h-[400px] w-full flex items-center justify-center">
			<!-- AWS Services Icons -->
			<div class="absolute inset-0">
				<svg width="100%" height="100%" viewBox="0 0 400 300" class="overflow-visible">
					<!-- Central RunsOn -->
					<g transform="translate(200, 150)">
						<circle cx="0" cy="0" r="40" fill="oklch(0.596 0.145 163.225)" opacity="0.2" stroke="oklch(0.596 0.145 163.225)" stroke-width="2"/>
						<text x="0" y="5" text-anchor="middle" fill="black" font-size="14" font-family="monospace" font-weight="bold">RunsOn</text>
					</g>
					
					<!-- EC2 -->
					<g transform="translate(80, 80)">
						<rect x="-30" y="-25" width="60" height="50" rx="4" fill="white" stroke="gray" stroke-width="1"/>
						<text x="0" y="-5" text-anchor="middle" fill="gray" font-size="11" font-family="monospace">EC2</text>
						<text x="0" y="10" text-anchor="middle" fill="gray" font-size="8" font-family="monospace">Compute</text>
					</g>
					<line x1="110" y1="105" x2="170" y2="135" stroke="oklch(0.596 0.145 163.225)" stroke-width="2" opacity="0.6"/>
					
					<!-- S3 -->
					<g transform="translate(320, 80)">
						<rect x="-30" y="-25" width="60" height="50" rx="4" fill="white" stroke="gray" stroke-width="1"/>
						<text x="0" y="-5" text-anchor="middle" fill="gray" font-size="11" font-family="monospace">S3</text>
						<text x="0" y="10" text-anchor="middle" fill="gray" font-size="8" font-family="monospace">Cache</text>
					</g>
					<line x1="290" y1="105" x2="230" y2="135" stroke="oklch(0.596 0.145 163.225)" stroke-width="2" opacity="0.6"/>
					
					<!-- CloudFormation -->
					<g transform="translate(80, 220)">
						<rect x="-30" y="-25" width="60" height="50" rx="4" fill="white" stroke="gray" stroke-width="1"/>
						<text x="0" y="-5" text-anchor="middle" fill="gray" font-size="9" font-family="monospace">CloudForm</text>
						<text x="0" y="10" text-anchor="middle" fill="gray" font-size="8" font-family="monospace">Deploy</text>
					</g>
					<line x1="110" y1="195" x2="170" y2="165" stroke="oklch(0.596 0.145 163.225)" stroke-width="2" opacity="0.6"/>
					
					<!-- Lambda -->
					<g transform="translate(320, 220)">
						<rect x="-30" y="-25" width="60" height="50" rx="4" fill="white" stroke="gray" stroke-width="1"/>
						<text x="0" y="-5" text-anchor="middle" fill="gray" font-size="11" font-family="monospace">Lambda</text>
						<text x="0" y="10" text-anchor="middle" fill="gray" font-size="8" font-family="monospace">Events</text>
					</g>
					<line x1="290" y1="195" x2="230" y2="165" stroke="oklch(0.596 0.145 163.225)" stroke-width="2" opacity="0.6"/>
				</svg>
			</div>
		</div>
	</div>
    
    <!-- Background Grid Pattern -->
    <div class="absolute inset-0 z-0 opacity-10" 
        style="background-image: linear-gradient(#ccc 1px, transparent 1px), linear-gradient(90deg, #ccc 1px, transparent 1px); background-size: 40px 40px;">
    </div>
</section>
