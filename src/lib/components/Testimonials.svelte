<script lang="ts">
	const testimonials = [
		{
			quote: "Less than 10 min to test, install and use the product. You can finetune any workflow depending on your needs. The cache download speed is blazing fast thanks to amazon s3 endpoint. Pricing is transparent, pay only what you use with no overage.",
			author: "Christopher Brookes",
			role: "SRE • Choose",
			image: "https://i.pravatar.cc/150?u=christopher",
            icon: "https://placehold.co/20x20/333/fff?text=C"
		},
		{
			quote: "We're in the process of moving from CircleCI to Github Actions. We've been using Actions Runner Controller on EKS, but hit a number of scaling issues, job pickup delays, and job cancellations. We started trialing RunsOn to see how other options might fair compared to ARC and have been thoroughly impressed.",
			author: "David Moran",
			role: "Lead DevSecOps Engineer • SmithRx",
			image: "https://i.pravatar.cc/150?u=david",
            icon: "https://placehold.co/20x20/000/fff?text=S"
		},
		{
			quote: "We've been using RunsOn for a short while and have already seen massive savings compared to using GH actions with larger runners. The ease of setup is also amazing, where it says on the website that it will take 10 minutes to setup I think that's understating how simple and quick it is to get going.",
			author: "Chad Lamb",
			role: "Software Engineer • RelyComply",
			image: "https://i.pravatar.cc/150?u=chad",
            icon: "https://placehold.co/20x20/purple/fff?text=R"
		},
		{
			quote: "RunsOn has been a game-changer for our CI/CD costs. The S3 caching is incredibly fast and the setup was straightforward. We're saving thousands per month.",
			author: "Alex Chen",
			role: "DevOps Lead • Tech Startup",
			image: "https://i.pravatar.cc/150?u=alex",
            icon: "https://placehold.co/20x20/blue/fff?text=T"
		},
		{
			quote: "The fact that it runs entirely in our AWS account was the deciding factor. No third-party access to our code, and we get full transparency. Plus the cost savings are incredible.",
			author: "Sarah Johnson",
			role: "CTO • FinTech Co",
			image: "https://i.pravatar.cc/150?u=sarah",
            icon: "https://placehold.co/20x20/green/fff?text=F"
		},
		{
			quote: "Setup took literally 10 minutes. The documentation is excellent and the CloudFormation stack just works. We're processing thousands of jobs daily with zero issues.",
			author: "Michael Torres",
			role: "Platform Engineer • Scale Corp",
			image: "https://i.pravatar.cc/150?u=michael",
            icon: "https://placehold.co/20x20/red/fff?text=S"
		}
	];
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto">
	<div class="text-center mb-16">
		<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
			[ TESTIMONIALS ]
		</span>
		<h2 class="font-display text-4xl md:text-5xl font-medium tracking-tight text-gray-900 mb-4">
			Trusted by 500+ Teams
		</h2>
		<p class="font-mono text-sm text-gray-600">
			See what DevOps engineers are saying about RunsOn
		</p>
	</div>

	<div class="columns-1 md:columns-2 lg:columns-3 gap-6 space-y-6">
		{#each testimonials as t}
			<div class="bg-white p-6 rounded-lg border border-gray-200 shadow-sm break-inside-avoid hover:shadow-md transition-shadow">
				<p class="font-mono text-xs leading-relaxed text-gray-700 mb-6">
					"{t.quote}"
				</p>
				<div class="flex items-center justify-between border-t border-gray-100 pt-4">
					<div class="flex items-center gap-3">
						<img src={t.image} alt={t.author} class="w-8 h-8 rounded-full bg-gray-200" />
						<div>
							<div class="text-xs font-bold text-gray-900">{t.author}</div>
							<div class="text-[10px] text-gray-500 font-mono">{t.role}</div>
						</div>
					</div>
                    <img src={t.icon} alt="Company Logo" class="w-5 h-5 rounded-sm opacity-70 grayscale" />
				</div>
			</div>
		{/each}
	</div>
</section>
