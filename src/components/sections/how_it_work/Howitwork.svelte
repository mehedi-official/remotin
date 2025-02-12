<script lang="ts">
	import Chip from '@components/Chip.svelte';
</script>

<section class=" p-24">
	<section
		class="mx-auto mb-10 grid max-w-lg justify-center justify-items-center gap-4 text-center"
	>
		<Chip>Our Process</Chip>
		<h2 class="text-5xl font-medium tracking-tighter text-[#1F1F1F]">How It Works</h2>
		<p class="px-12 text-base tracking-tight text-gray-600">
			Get Remote Workers Ready in 3 Simple Steps.
		</p>
	</section>

	<section class="grid grid-cols-3 gap-4">
		<article class="rounded-lg border-2 border-[#EAE9FB] p-1">
			<div class="grid gap-5 bg-[#FCFBFF] p-3">
				<div class="h-10 w-10 rounded-full bg-[#EAECFE]"></div>

				<div class="grid gap-3 text-center">
					<h3 class="text-base/4 font-medium text-[#1f1f1f]">
						Initial Consultation: Understand Your Needs
					</h3>
					<p class="text-sm tracking-tight text-gray-600">
						We start by listening to your business needs. We make sure every detail is understood.
					</p>
				</div>
			</div>
		</article>

		<article class="rounded-lg border-2 border-[#EAE9FB] p-1">
			<div class="grid gap-5 bg-[#FCFBFF] p-3">
				<div class="h-10 w-10 rounded-full bg-[#EAECFE]"></div>

				<div class="grid gap-3 text-center">
					<h3 class="text-base/4 font-medium text-[#1f1f1f]">Fast and Efficient Onboarding</h3>
					<p class="text-sm tracking-tight text-gray-600">
						We ensure all the tools and information needed are available from day one.
					</p>
				</div>
			</div>
		</article>

		<article class="rounded-lg border-2 border-[#EAE9FB] p-1">
			<div class="grid gap-5 bg-[#FCFBFF] p-3">
				<div class="h-10 w-10 rounded-full bg-[#EAECFE]"></div>

				<div class="grid gap-3 text-center">
					<h3 class="text-base/4 font-medium text-[#1f1f1f]">Ongoing monitoring and support</h3>
					<p class="text-sm tracking-tight text-gray-600">
						We provide full support to ensure the collaboration runs smoothly.
					</p>
				</div>
			</div>
		</article>
	</section>
</section>
