<script lang="ts">
	import { facebook, instagram, linkedin, twitter } from '@components/Logos.svelte';

	let social_icons = $state([facebook, linkedin, instagram, twitter]);
</script>

<footer class="bg-[#020202] px-12 text-[#F0F0F0]">
	<section class=" grid grid-cols-2 gap-6 py-[4.5rem]">
		<div class="inline-grid gap-6">
			<h3 class=" pr-12 text-[2.5rem]/[130%] font-medium tracking-tighter">
				Budget Saving, high flexibility and effectiveness. Start getting them now.
			</h3>
			<button
				class="inline-flex w-fit rounded-md bg-white px-4 py-[10px] text-sm/[14px] font-semibold text-[#020202]"
				>Get Started</button
			>
		</div>

		<div class="flex justify-between">
			<div>
				<h4 class="mb-6 text-base/4 font-medium tracking-tight">Navigation</h4>
				<ul class=" grid gap-4 text-sm/[14px] font-light tracking-tight">
					<li class=" underline-offset-4 hover:underline"><a href="/">Home</a></li>
					<li class=" underline-offset-4 hover:underline"><a href="/">Tools</a></li>
					<li class=" underline-offset-4 hover:underline"><a href="/">About Us</a></li>
					<li class=" underline-offset-4 hover:underline"><a href="/">Pricing</a></li>
					<li class=" underline-offset-4 hover:underline"><a href="/">Services</a></li>
					<li class=" underline-offset-4 hover:underline"><a href="/">Contact Us</a></li>
				</ul>
			</div>

			<div>
				<h4 class="mb-6 text-base/4 font-medium tracking-tight">Company</h4>
				<ul class=" grid gap-4 text-sm/[14px] font-light tracking-tight">
					<li class=" underline-offset-4 hover:underline"><a href="/">News</a></li>
					<li class=" underline-offset-4 hover:underline"><a href="/">Career</a></li>
					<li class=" underline-offset-4 hover:underline"><a href="/">Our Story</a></li>
				</ul>
			</div>

			<div>
				<h4 class="mb-6 text-base/4 font-medium tracking-tight">Most Frequently Employed</h4>
				<ul class=" grid gap-4 text-sm/[14px] font-light tracking-tight">
					<li class=" underline-offset-4 hover:underline"><a href="/">Software Engineer</a></li>
					<li class=" underline-offset-4 hover:underline"><a href="/">Graphic Designer</a></li>
					<li class=" underline-offset-4 hover:underline"><a href="/">UI Design</a></li>
					<li class=" underline-offset-4 hover:underline"><a href="/">UX Design</a></li>
					<li class=" underline-offset-4 hover:underline"><a href="/">Web Programmer</a></li>
				</ul>
			</div>
		</div>
	</section>
	<section class=" flex items-center justify-between py-9">
		<p class=" text-base/4 font-light tracking-tight">
			©{new Date().getFullYear()} Remotin. All rights reserved. Developed by
			<a
				class=" font-medium text-white underline underline-offset-4"
				href="https://mehedi-agency.vercel.app"
				target="_blank"><strong>Mehedi Hasan</strong></a
			>.
		</p>
		<div class="flex items-center gap-4">
			{#each social_icons as social}
				<div>{@render social()}</div>
			{/each}
		</div>
	</section>
</footer>
