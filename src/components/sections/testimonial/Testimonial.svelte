<script>
	import testimonial_img from '$lib/assets/testimonial.png';
	import Chip from '@components/Chip.svelte';
	import avatar_01 from '$lib/assets/avatar_01.png';
</script>

<section>
	<section
		class="mx-auto mb-10 grid max-w-[36rem] justify-center justify-items-center gap-4 text-center"
	>
		<Chip>Testimonial</Chip>
		<h2 class="text-5xl font-medium tracking-tighter text-[#1F1F1F]">What People Say About Us</h2>
		<p class="px-12 text-base tracking-tight text-gray-600">
			Their satisfaction is all thanks to our hard work. Check out their testimonials.
		</p>
	</section>

	<section class="content px-48">
		<article class="first rounded-lg border-2 border-[#EAE9FB] p-1">
			<div class="flex h-full flex-col justify-between gap-5 bg-[#FCFBFF] p-3">
				<p class="text-base tracking-tight text-gray-600">
					"Remotin made it so easy for us to build a global team.We found top-notch professionals
					who fit perfectly with our company culture. The process was fast, and the results have
					been outstanding!"
				</p>
				<div class="flex items-center gap-3">
					<div class="h-8 w-8 overflow-hidden rounded-md">
						<img class="h-full w-full" src={avatar_01} alt="Lilin Herlina" />
					</div>
					<div class="grid gap-1">
						<h4 class=" text-xs/3 font-semibold text-[#1F1F1F]">Pablo Hernandez</h4>
						<p class=" text-xs/3 font-normal text-gray-600">Founder, Bikana Creative Studio</p>
					</div>
				</div>
			</div>
		</article>

		<article class="second rounded-lg border-2 border-[#EAE9FB] p-1">
			<div class="flex h-full flex-col justify-between gap-5 bg-[#FCFBFF] p-3">
				<p class="text-base tracking-tight text-gray-600">
					"Our startup required a flexible workforce for short-term projects, and Remotin delivered
					exactly whatwe needed. Their remote workers areskilled, responsive, and highly adaptable."
				</p>
				<div class="flex items-center gap-3">
					<div class="h-8 w-8 overflow-hidden rounded-md">
						<img class="h-full w-full" src={avatar_01} alt="Lilin Herlina" />
					</div>
					<div class="grid gap-1">
						<h4 class=" text-xs/3 font-semibold text-[#1F1F1F]">Lilin Herlina</h4>
						<p class=" text-xs/3 font-normal text-gray-600">Product Manager at Hublot</p>
					</div>
				</div>
			</div>
		</article>

		<article class="middle overflow-hidden rounded-lg">
			<img class="h-full w-full" src={testimonial_img} alt="Testimonial of Orix Agency" />
		</article>

		<article class="third rounded-lg border-2 border-[#EAE9FB] p-1">
			<div class="flex h-full flex-col justify-between gap-5 bg-[#FCFBFF] p-3">
				<p class="text-base tracking-tight text-gray-600">
					"Hiring through Remotin has been a game-changer for our business. We've significantly
					reduced operational costs while maintaining high-quality output. Their support team is
					always there when we need them."
				</p>
				<div class="flex items-center gap-3">
					<div class="h-8 w-8 overflow-hidden rounded-md">
						<img class="h-full w-full" src={avatar_01} alt="Lilin Herlina" />
					</div>
					<div class="grid gap-1">
						<h4 class=" text-xs/3 font-semibold text-[#1F1F1F]">James Lee</h4>
						<p class=" text-xs/3 font-normal text-gray-600">Founder of BrightStart Marketing</p>
					</div>
				</div>
			</div>
		</article>

		<article class=" fourth rounded-lg border-2 border-[#EAE9FB] p-1">
			<div class="flex h-full flex-col justify-between gap-5 bg-[#FCFBFF] p-3">
				<p class="text-base tracking-tight text-gray-600">
					"With Remotin, we've hired amazing talent from different time zones. It's incredible how
					smoothly they integrate into our workflows. Highly recommend their services!"
				</p>
				<div class="flex items-center gap-3">
					<div class="h-8 w-8 overflow-hidden rounded-md">
						<img class="h-full w-full" src={avatar_01} alt="Lilin Herlina" />
					</div>
					<div class="grid gap-1">
						<h4 class=" text-xs/3 font-semibold text-[#1F1F1F]">Ankit Sutrapranal</h4>
						<p class=" text-xs/3 font-normal text-gray-600">Operations Lead at Globalreach</p>
					</div>
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
			'first middle second'
			'third middle fourth';
		grid-template-columns: 2fr 3fr 2fr;
	}

	.first {
		grid-area: first;
	}

	.second {
		grid-area: second;
	}

	.third {
		grid-area: third;
	}

	.middle {
		grid-area: middle;
	}

	.fourth {
		grid-area: fourth;
	}
</style>
