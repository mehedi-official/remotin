<script lang="ts">
	import { logo } from '@components/Logos.svelte';
</script>

<nav
	class="box-border flex items-center justify-between border-b border-[#F0F0F0] px-4 py-4 lg:px-24 lg:py-0"
>
	<section class="flex items-center gap-16">
		<div>{@render logo()}</div>
		<ul
			class="hidden items-center gap-10 text-base/4 font-medium tracking-tight text-[#3E3E3E] lg:flex"
		>
			<li class="border-y-2 border-transparent py-6 hover:border-b-[#5C43DC]">
				<a href="/">Overview</a>
			</li>
			<li class="border-y-2 border-transparent py-6 hover:border-b-[#5C43DC]">
				<a href="/">Tools</a>
			</li>
			<li class="border-y-2 border-transparent py-6 hover:border-b-[#5C43DC]">
				<a href="/">About Us</a>
			</li>
			<li class="border-y-2 border-transparent py-6 hover:border-b-[#5C43DC]">
				<a href="/">Pricing</a>
			</li>
			<li class="border-y-2 border-transparent py-6 hover:border-b-[#5C43DC]">
				<a href="/">Services</a>
			</li>
		</ul>
	</section>

	<div class="flex gap-3">
		<button
			class="hidden rounded-md border border-[#E9E9E9] px-3 py-[10px] text-sm/[14px] font-semibold text-[#1F1F1F] hover:bg-slate-50 lg:block"
			>Learn More</button
		>
		<button
			class="rounded-md bg-[#5254D3] px-3 py-[10px] text-sm/[14px] font-semibold text-white hover:bg-[#373ac7]"
			>Get Started</button
		>
	</div>
</nav>
