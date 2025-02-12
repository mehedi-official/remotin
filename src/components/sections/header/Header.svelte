<script lang="ts">
	import { star } from '@components/Icons.svelte';
	import Navbar from './Navbar.svelte';
	import avatar_01 from '$lib/assets/avatar_01.png';
	import avatar_02 from '$lib/assets/avatar_02.png';
	import avatar_03 from '$lib/assets/avatar_03.png';

	let avatars = [avatar_01, avatar_02, avatar_03];
</script>

<header>
	<Navbar />

	<section class="grid grid-cols-2 px-24 py-16">
		<section>
			<div class="mb-20 grid gap-5">
				<h1 class=" text-[3.25rem]/[130%] font-medium tracking-tighter text-[#1F1F1F]">
					Present <span class="text-[#5856C2]">Remote Workers</span> as the Best Assistants for Your
					Work.
				</h1>
				<p class="pr-24 text-base tracking-tight text-gray-600">
					Find talented professionals from around the world who are ready to help your business grow
					without geographical boundaries.
				</p>

				<div>
					<button
						class="rounded-md bg-[#5254D3] px-4 py-[10px] text-sm/[14px] font-semibold text-white"
						>Get Started</button
					>
					<button
						class="rounded-md border border-[#E9E9E9] px-4 py-[10px] text-sm/[14px] font-semibold"
						>How it Works</button
					>
				</div>
			</div>

			<div class="flex items-center gap-3">
				<div class="flex">
					{#each avatars as avatar, i}
						<div class={['overflow-hidden rounded-full border-2 border-white', i !== 0 && '-ml-3']}>
							<img src={avatar} alt="avatar_{i + 1}" />
						</div>
					{/each}
				</div>

				<div>
					<div class="flex items-center gap-2">
						{#each { length: 5 }}
							<span>{@render star()}</span>
						{/each}
						<span class="text-secondary text-sm/[14px] font-semibold">(5.0)</span>
					</div>
					<p class="mt-1 text-sm/[14px] font-normal text-gray-400">from 5000 reviewers</p>
				</div>
			</div>
		</section>

		<section></section>
	</section>
</header>
