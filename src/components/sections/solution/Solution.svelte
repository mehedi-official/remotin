<script lang="ts">
	import Chip from '@components/Chip.svelte';
	import { cost_saving, world_quality, flexible_hour } from '@components/Icons.svelte';
</script>

<section class=" px-4 lg:p-24">
	<section class="flex flex-col items-end justify-between gap-8 lg:flex-row lg:gap-16">
		<div class="inline-grid gap-4">
			<Chip>How We Help You</Chip>
			<h2
				class=" max-w-[34rem] text-4xl font-medium leading-tight tracking-tighter text-[#1F1F1F] lg:text-5xl"
			>
				Maximize your business potential with the best remote worker
			</h2>
		</div>
		<p class=" max-w-96 text-sm tracking-tight text-gray-600 lg:text-base">
			We connect you with skilled talent tailored to your unique needs, ensuring quality, efficiency
			and cost-effectiveness for your project.
		</p>
	</section>

	<section class="content mt-12">
		<article class="first rounded-lg border-2 border-[#EAE9FB] p-1">
			<div class="flex h-full flex-col justify-between gap-12 bg-[#FCFBFF] p-3">
				<div class="mx-auto mt-9 flex h-[20.5rem] max-w-[20.625rem] justify-center">
					{@render cost_saving()}
				</div>

				<div class="grid gap-3 text-center">
					<h3 class="text-base/4 font-medium text-[#1f1f1f]">Cost Saving</h3>
					<p class="text-sm tracking-tight text-gray-600">
						No need to provide office space, equipment, or physical infrastructure. With a remote
						team, you immediately reduce rental costs.
					</p>
				</div>
			</div>
		</article>

		<article class="second rounded-lg border-2 border-[#EAE9FB] p-1">
			<div class="grid gap-5 bg-[#FCFBFF] p-3">
				<div class="mx-auto mt-9 flex h-[10.375rem] max-w-[21.125rem] justify-center">
					{@render world_quality()}
				</div>

				<div class="grid gap-3 text-center">
					<h3 class="text-base/4 font-medium text-[#1f1f1f]">World-Class Quality</h3>
					<p class="text-sm tracking-tight text-gray-600">
						Remote workers allow you to work with world-class professionals who are ready to deliver
						high-quality results for every project you have.
					</p>
				</div>
			</div>
		</article>

		<article class="third rounded-lg border-2 border-[#EAE9FB] p-1">
			<div
				class="flex flex-col items-center gap-8 bg-[#FCFBFF] px-4 py-4 lg:flex-row lg:px-12 lg:py-10"
			>
				<div class="mx-auto flex h-[12.25rem] min-w-[11.125rem] justify-center">
					{@render flexible_hour()}
				</div>

				<div class="grid gap-3">
					<h3 class="text-base/4 font-medium text-[#1f1f1f]">Flexible Hours</h3>
					<p class="text-sm tracking-tight text-gray-600">
						With our workforce, working hours are no longer a limitation. Remote workers can work
						according to their productive hours, ensuring the best results without compromise.
					</p>
				</div>
			</div>
		</article>
	</section>
</section>

<style>
	.content {
		display: grid;
		gap: 1rem;
		grid-template-areas:
			'side'
			'main-1'
			'main-2';

		grid-template-columns: 1fr;
		grid-template-rows: 1fr;
	}

	@media (min-width: 64rem) {
		.content {
			display: grid;
			grid-template-areas:
				'side main-1'
				'side main-2';
			grid-template-columns: 1fr 1fr;
		}
	}

	.first {
		grid-area: side;
	}

	.second {
		grid-area: main-1;
	}

	.third {
		grid-area: main-2;
	}
</style>
