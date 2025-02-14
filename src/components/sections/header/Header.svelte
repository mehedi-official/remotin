<script lang="ts">
	import { star } from '@components/Icons.svelte';
	import Navbar from './Navbar.svelte';
	import hero_img from '$lib/assets/hero_img.png?enhanced';
	import avatar_01 from '$lib/assets/avatar_01.png';
	import avatar_02 from '$lib/assets/avatar_02.png';
	import avatar_03 from '$lib/assets/avatar_03.png';

	let avatars = [avatar_01, avatar_02, avatar_03];
</script>

<header>
	<Navbar />

	<section class="grid gap-8 px-4 py-16 lg:grid-cols-2 lg:px-24">
		<section class="flex flex-col justify-between">
			<div class="mt-5 grid gap-5">
				<h1
					class=" text-4xl/[130%] font-medium tracking-tighter text-[#1F1F1F] lg:text-[3.25rem]/[130%]"
				>
					Present <span class="text-[#5254D3]">Remote Workers</span> as the Best Assistants for Your
					Work.
				</h1>
				<p class="text-base tracking-tight text-gray-600 lg:pr-24">
					Find talented professionals from around the world who are ready to help your business grow
					without geographical boundaries.
				</p>

				<div>
					<button
						class="rounded-md bg-[#5254D3] px-4 py-[10px] text-sm/[14px] font-semibold text-white hover:bg-[#373ac7]"
						>Get Started</button
					>
					<button
						class="rounded-md border border-[#E9E9E9] px-4 py-[10px] text-sm/[14px] font-semibold hover:bg-slate-50"
						>How it Works</button
					>
				</div>
			</div>

			<div class=" mb-5 mt-8 flex items-center gap-3 lg:mt-0">
				<div class="flex">
					{#each avatars as avatar, i}
						<div
							class={[
								'h-10 w-10 overflow-hidden rounded-full border-2 border-white',
								i !== 0 && '-ml-3'
							]}
						>
							<img class="h-full w-full" src={avatar} alt="avatar_{i + 1}" />
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

		<section class=" lg:pl-20">
			<div class="overflow-hidden rounded-2xl">
				<enhanced:img src={hero_img} alt="Hero Banner" />
			</div>
		</section>
	</section>
</header>
