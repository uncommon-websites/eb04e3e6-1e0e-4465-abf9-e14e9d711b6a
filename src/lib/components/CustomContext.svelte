<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto">
	<div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-center">
		<div>
			<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
				[ SIMPLE CONFIGURATION ]
			</span>
			<h2 class="font-display text-4xl md:text-5xl lg:text-6xl font-medium tracking-tight text-gray-900 mb-6 leading-[0.95]">
				Setup in<br>10 minutes.
			</h2>
			<p class="font-mono text-sm text-gray-600 max-w-md mb-12">
				Get started with RunsOn in three simple steps. No complex Kubernetes setup required.
			</p>

			<div class="space-y-12 relative">
                <!-- Vertical line connecting steps -->
                <div class="absolute left-[11px] top-2 bottom-2 w-[1px] bg-gray-200 -z-10"></div>

				<div class="flex gap-6 group">
					<div class="w-6 h-6 rounded-full bg-brand-green border border-brand-green flex items-center justify-center text-xs font-mono text-white shrink-0 shadow-sm">1</div>
					<div>
						<h3 class="font-bold text-gray-900 mb-2">Deploy CloudFormation stack</h3>
						<p class="text-sm text-gray-600 leading-relaxed max-w-sm">
							One-click CloudFormation deployment sets up all AWS resources in your account.
						</p>
					</div>
				</div>

				<div class="flex gap-6 group">
					<div class="w-6 h-6 rounded-full bg-gray-100 border border-gray-300 flex items-center justify-center text-xs font-mono text-gray-500 shrink-0 group-hover:bg-brand-green group-hover:border-brand-green group-hover:text-white transition-colors">2</div>
					<div>
						<h3 class="font-bold text-gray-900 mb-2">Add license key to GitHub secrets</h3>
						<p class="text-sm text-gray-600 leading-relaxed max-w-sm">
							Store your RunsOn license key as a GitHub secret for authentication.
						</p>
					</div>
				</div>

				<div class="flex gap-6 group">
					<div class="w-6 h-6 rounded-full bg-gray-100 border border-gray-300 flex items-center justify-center text-xs font-mono text-gray-500 shrink-0 group-hover:bg-brand-green group-hover:border-brand-green group-hover:text-white transition-colors">3</div>
					<div>
						<h3 class="font-bold text-gray-900 mb-2">Update your workflow YAML</h3>
						<p class="text-sm text-gray-600 leading-relaxed max-w-sm">
							Change <code class="bg-gray-100 px-1 py-0.5 rounded text-xs">runs-on: ubuntu-latest</code> to <code class="bg-gray-100 px-1 py-0.5 rounded text-xs">runs-on: runs-on/runner=2cpu-linux</code>
						</p>
					</div>
				</div>
			</div>
			
			<div class="mt-12">
				<a href="https://runs-on.com/guides/getting-started" class="bg-black text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-gray-800 transition-colors flex items-center gap-2 font-mono uppercase tracking-wide text-xs w-fit">
					View setup guide ->
				</a>
			</div>
		</div>

		<div class="bg-[#F3F3F1] p-2 rounded-lg border border-gray-200 shadow-sm">
            <div class="bg-gray-900 rounded border border-gray-700 overflow-hidden p-6">
				<!-- Code snippet -->
				<div class="font-mono text-xs text-gray-300 space-y-2">
					<div class="text-gray-500"># .github/workflows/ci.yml</div>
					<div><span class="text-blue-400">name:</span> CI</div>
					<div><span class="text-blue-400">on:</span> [push]</div>
					<div class="mt-4"><span class="text-blue-400">jobs:</span></div>
					<div class="ml-4"><span class="text-blue-400">test:</span></div>
					<div class="ml-8"><span class="text-green-400">runs-on:</span> runs-on/runner=2cpu-linux</div>
					<div class="ml-8"><span class="text-blue-400">steps:</span></div>
					<div class="ml-12">- <span class="text-blue-400">uses:</span> actions/checkout@v4</div>
					<div class="ml-12">- <span class="text-blue-400">run:</span> npm test</div>
				</div>
            </div>
		</div>
	</div>
</section>
