<script lang="ts">
	import { building, check_fill, star } from '@components/Icons.svelte';
	import PricingCard from './PricingCard.svelte';
	import Chip from '@components/Chip.svelte';
</script>

<section>
	<section
		class="mb-10 mt-32 grid max-w-lg gap-4 px-4 lg:mx-auto lg:mt-0 lg:justify-center lg:justify-items-center lg:text-center"
	>
		<Chip>Pricing</Chip>
		<h2 class=" text-4xl font-medium tracking-tighter text-[#1F1F1F] lg:text-5xl">
			Plans that fit your needs, pricing that's fair
		</h2>
		<p class="text-sm tracking-tight text-gray-600 lg:px-12 lg:text-base">
			Pay only for what you need, with transparent pricing and no hidden fees.
		</p>
	</section>

	<section class="mb-32 flex flex-col justify-center gap-7 px-4 lg:flex-row">
		<PricingCard>
			{#snippet category()}
				<span class="inline-flex items-center gap-2">{@render star('#2A42CB')}Starter Plan</span>
			{/snippet}

			{#snippet header()}
				<div class="inline-grid gap-3">
					<h3 class=" text-[2rem]/[2rem] font-semibold text-[#98989C]">
						$<span class="text-[#1f1f1f]">6,000 </span><span class=" text-sm/[14px] font-normal"
							>/month</span
						>
					</h3>
					<p class=" text-sm/[14px] font-medium tracking-tight text-[#1f1f1f]">
						✨ Perfect for small teams.
					</p>
				</div>
			{/snippet}

			{#snippet benefit()}
				<p class="flex items-center gap-2 text-sm/[14px] font-normal text-[#45474D]">
					{@render check_fill()} Access to pre-vetted remote workers.
				</p>
				<p class="flex items-center gap-2 text-sm/[14px] font-normal text-[#45474D]">
					{@render check_fill()} Up to 5 active job posting.
				</p>
				<p class="flex items-center gap-2 text-sm/[14px] font-normal text-[#45474D]">
					{@render check_fill()} Default Analytics dashboard.
				</p>
				<p class="flex items-center gap-2 text-sm/[14px] font-normal text-[#45474D]">
					{@render check_fill()} 24/7 Priorty support.
				</p>
			{/snippet}
		</PricingCard>

		<PricingCard>
			{#snippet category()}
				<span class="inline-flex items-center gap-2">{@render building()}Enterprise Plan</span>
			{/snippet}

			{#snippet header()}
				<div class="inline-grid gap-3">
					<h3 class=" text-[2rem]/[2rem] font-semibold text-[#98989C]">
						$<span class="text-[#1f1f1f]">9,000 </span><span class=" text-sm/[14px] font-normal"
							>/month</span
						>
					</h3>
					<p class=" text-sm/[14px] font-medium tracking-tight text-[#1f1f1f]">
						✨ Perfect for startup & large teams.
					</p>
				</div>
			{/snippet}

			{#snippet benefit()}
				<p class="flex items-center gap-2 text-sm/[14px] font-normal text-[#45474D]">
					{@render check_fill()} Custom talent sourcing.
				</p>
				<p class="flex items-center gap-2 text-sm/[14px] font-normal text-[#45474D]">
					{@render check_fill()} Unlimited job postings.
				</p>
				<p class="flex items-center gap-2 text-sm/[14px] font-normal text-[#45474D]">
					{@render check_fill()} Advanced Analytics dashboard.
				</p>
				<p class="flex items-center gap-2 text-sm/[14px] font-normal text-[#45474D]">
					{@render check_fill()} 24/7 Priorty support.
				</p>
			{/snippet}
		</PricingCard>
	</section>
</section>
