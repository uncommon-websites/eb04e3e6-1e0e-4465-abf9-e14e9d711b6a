<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto relative overflow-hidden">
	<div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center relative z-10">
		<div>
			<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
				[ MAGIC CACHE ]
			</span>
			<h2 class="font-display text-4xl md:text-5xl lg:text-6xl font-medium tracking-tight text-gray-900 mb-6 leading-[0.95]">
				5x faster<br>than GitHub.
			</h2>
			<p class="font-mono text-sm text-gray-600 max-w-md mb-8 leading-relaxed">
				RunsOn's transparent S3-based caching is 5x faster than GitHub's cache. Plus EBS snapshot-based block-level caching for Docker images. Zero configuration required.
			</p>
			
			<a href="https://runs-on.com/docs/caching" class="bg-black text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-gray-800 transition-colors flex items-center gap-2 font-mono uppercase tracking-wide text-xs w-fit">
				<span class="text-brand-green">⚡</span> Learn about caching
			</a>
		</div>

		<div class="relative h-[400px] w-full flex items-center justify-center">
			<!-- Background Text Pattern -->
            <div class="absolute inset-0 flex flex-col items-center justify-center opacity-5 select-none pointer-events-none overflow-hidden leading-none">
                {#each Array(10) as _, i}
                    <div class="text-6xl md:text-8xl font-black text-gray-900 whitespace-nowrap">
                        CACHE CACHE CACHE CACHE
                    </div>
                {/each}
            </div>

            <!-- Floating Cards -->
            <div class="relative z-10 flex flex-col gap-4 w-full max-w-md">
                <div class="bg-white p-4 rounded shadow-lg border border-gray-200 transform -rotate-2 translate-x-4">
                    <div class="flex items-center gap-2 mb-2">
                        <span class="bg-brand-green text-white text-[10px] font-bold px-1.5 py-0.5 rounded uppercase">S3 Cache</span>
                        <span class="text-xs text-gray-500">5x faster</span>
                    </div>
                    <p class="text-sm font-mono text-gray-800">Transparent caching via S3 endpoint</p>
                </div>

                <div class="bg-white p-4 rounded shadow-lg border border-gray-200 transform rotate-1 translate-x-8">
                    <div class="flex items-center gap-2 mb-2">
                        <span class="bg-accent-orange text-white text-[10px] font-bold px-1.5 py-0.5 rounded uppercase">EBS Snapshots</span>
                        <span class="text-xs text-gray-500">Block-level</span>
                    </div>
                    <p class="text-sm font-mono text-gray-800">Docker layer caching at block level</p>
                </div>

                 <div class="bg-white p-4 rounded shadow-lg border border-gray-200 transform -rotate-1">
                    <div class="flex items-center gap-2 mb-2">
                        <span class="bg-accent-pink text-white text-[10px] font-bold px-1.5 py-0.5 rounded uppercase">ECR Registry</span>
                        <span class="text-xs text-gray-500">Ephemeral</span>
                    </div>
                    <p class="text-sm font-mono text-gray-800">Automatic cleanup & cost optimization</p>
                </div>
            </div>
		</div>
	</div>
</section>
