<script lang="ts">
	import {
		creative,
		enterprise,
		freelancer,
		global,
		home,
		monitor
	} from '@components/Icons.svelte';
</script>

<section class="grid gap-4 lg:grid-cols-3">
	<article class="rounded-lg border-2 border-[#EAE9FB] p-1">
		<div class="grid gap-5 bg-[#FCFBFF] p-3">
			<div class="flex h-10 w-10 items-center justify-center rounded-full bg-[#EAECFE]">
				{@render monitor()}
			</div>

			<div class="grid gap-3">
				<h3 class="text-lg/5 font-medium text-[#212121]">IT Company</h3>
				<p class="text-sm tracking-tight text-gray-600">
					Get the best remote talent in technology from software developers, data analysts to
					cybersecurity experts, ready to support your innovation.
				</p>
			</div>
		</div>
	</article>

	<article class="rounded-lg border-2 border-[#EAE9FB] p-1">
		<div class="grid gap-5 bg-[#FCFBFF] p-3">
			<div class="flex h-10 w-10 items-center justify-center rounded-full bg-[#EAECFE]">
				{@render home()}
			</div>

			<div class="grid gap-3">
				<h3 class="text-lg/5 font-medium text-[#212121]">Startup</h3>
				<p class="text-sm tracking-tight text-gray-600">
					With Remotin, you can get experienced professionals without having to burden your
					operational budget. Save time and money.
				</p>
			</div>
		</div>
	</article>

	<article class="rounded-lg border-2 border-[#EAE9FB] p-1">
		<div class="grid gap-5 bg-[#FCFBFF] p-3">
			<div class="flex h-10 w-10 items-center justify-center rounded-full bg-[#EAECFE]">
				{@render enterprise()}
			</div>

			<div class="grid gap-3">
				<h3 class="text-lg/5 font-medium text-[#212121]">Enterprise Teams</h3>
				<p class="text-sm tracking-tight text-gray-600">
					Streamline your hiring process and scale with tailored solutions for large scale
					operations. Perfect for teams expanding across multiple locations.
				</p>
			</div>
		</div>
	</article>

	<article class="rounded-lg border-2 border-[#EAE9FB] p-1">
		<div class="grid gap-5 bg-[#FCFBFF] p-3">
			<div class="flex h-10 w-10 items-center justify-center rounded-full bg-[#EAECFE]">
				{@render freelancer()}
			</div>

			<div class="grid gap-3">
				<h3 class="text-lg/5 font-medium text-[#212121]">Freelancers</h3>
				<p class="text-sm tracking-tight text-gray-600">
					Leave operational tasks to our remote workers and focus on building strategies and
					innovations to grow your business.
				</p>
			</div>
		</div>
	</article>

	<article class="rounded-lg border-2 border-[#EAE9FB] p-1">
		<div class="grid gap-5 bg-[#FCFBFF] p-3">
			<div class="flex h-10 w-10 items-center justify-center rounded-full bg-[#EAECFE]">
				{@render global()}
			</div>

			<div class="grid gap-3">
				<h3 class="text-lg/5 font-medium text-[#212121]">Global Team</h3>
				<p class="text-sm tracking-tight text-gray-600">
					Building a high quality team is no longer limited by geographical location. With Remotin,
					you can recruit from all over the world.
				</p>
			</div>
		</div>
	</article>

	<article class="rounded-lg border-2 border-[#EAE9FB] p-1">
		<div class="grid gap-5 bg-[#FCFBFF] p-3">
			<div class="flex h-10 w-10 items-center justify-center rounded-full bg-[#EAECFE]">
				{@render creative()}
			</div>

			<div class="grid gap-3">
				<h3 class="text-lg/5 font-medium text-[#212121]">Creative Agencies</h3>
				<p class="text-sm tracking-tight text-gray-600">
					With a team of professionals from all over the world, we deliver the best creative
					solution to meet your's brand need.
				</p>
			</div>
		</div>
	</article>
</section>
