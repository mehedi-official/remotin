<script lang="ts">
	import Chip from '@components/Chip.svelte';
	import { consultation, monitoring, onboarding } from '@components/Icons.svelte';
</script>

<section class="px-4 py-8 lg:p-24">
	<section
		class="mb-10 mt-24 grid max-w-lg gap-4 lg:mx-auto lg:mt-0 lg:justify-center lg:justify-items-center lg:text-center"
	>
		<Chip>Our Process</Chip>
		<h2 class=" text-4xl font-medium tracking-tighter text-[#1F1F1F] lg:text-5xl">How It Works</h2>
		<p class="text-sm tracking-tight text-gray-600 lg:px-12 lg:text-base">
			Get Remote Workers Ready in 3 Simple Steps.
		</p>
	</section>

	<section class="grid gap-4 lg:grid-cols-3">
		<article class="rounded-lg border-2 border-[#EAE9FB] p-1">
			<div class="grid gap-5 bg-[#FCFBFF] p-3">
				<div
					class="flex h-10 w-10 items-center justify-center rounded-md border border-[#EEEDF0] bg-[#FCFCF9] text-base/4 font-bold text-[#2741D8]"
				>
					01
				</div>

				<div class="mb-4 flex -translate-y-8 justify-center">
					{@render consultation()}
				</div>

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
				<div
					class="flex h-10 w-10 items-center justify-center rounded-md border border-[#EEEDF0] bg-[#FCFCF9] text-base/4 font-bold text-[#2741D8]"
				>
					02
				</div>

				<div class="mb-4 flex -translate-y-8 justify-center">
					{@render onboarding()}
				</div>

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
				<div
					class="flex h-10 w-10 items-center justify-center rounded-md border border-[#EEEDF0] bg-[#FCFCF9] text-base/4 font-bold text-[#2741D8]"
				>
					03
				</div>

				<div class="mb-4 flex -translate-y-8 justify-center">
					{@render monitoring()}
				</div>

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
