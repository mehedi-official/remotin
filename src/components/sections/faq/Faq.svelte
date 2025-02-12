<script lang="ts">
	import Chip from '@components/Chip.svelte';
	import { arrow_down } from '@components/Icons.svelte';
	import { slide } from 'svelte/transition';

	let questions_1 = $state([
		{
			question: 'What is Remotin?',
			answer:
				'Remotin is a platform that connects businesses with top-tier remote professionals from around the world. We specialize in providing pre-vetted talent for a wide range of industries and roles.',
			isActive: false
		},
		{
			question: 'How do you vet remote workers?',
			answer:
				'Remotin is a platform that connects businesses with top-tier remote professionals from around the world. We specialize in providing pre-vetted talent for a wide range of industries and roles.',
			isActive: false
		},
		{
			question: 'What types of roles can I hire for through Remotin?',
			answer:
				'Remotin is a platform that connects businesses with top-tier remote professionals from around the world. We specialize in providing pre-vetted talent for a wide range of industries and roles.',
			isActive: false
		}
	]);

	let questions_2 = $state([
		{
			question: 'How quickly can I hire a remote worker?',
			answer:
				'Remotin is a platform that connects businesses with top-tier remote professionals from around the world. We specialize in providing pre-vetted talent for a wide range of industries and roles.',
			isActive: false
		},
		{
			question: 'Can I hire on a part-time or project basis?',
			answer:
				'Remotin is a platform that connects businesses with top-tier remote professionals from around the world. We specialize in providing pre-vetted talent for a wide range of industries and roles.',
			isActive: false
		},
		{
			question: 'What if I am not satisfied with a remote worker?',
			answer:
				'Remotin is a platform that connects businesses with top-tier remote professionals from around the world. We specialize in providing pre-vetted talent for a wide range of industries and roles.',
			isActive: false
		},
		{
			question: 'Is there ongoing support for managing remote worker?',
			answer:
				'Remotin is a platform that connects businesses with top-tier remote professionals from around the world. We specialize in providing pre-vetted talent for a wide range of industries and roles.',
			isActive: false
		}
	]);

	function handleAccordian(group: string, idx: number) {
		if (group === 'group_1') {
			questions_1[idx].isActive = !questions_1[idx].isActive;
		} else if (group === 'group_2') {
			questions_2[idx].isActive = !questions_2[idx].isActive;
		}
	}
</script>

<section class="p-24">
	<section class="flex flex-col items-center gap-4 text-center">
		<Chip>Frequently Asked Question</Chip>
		<h2 class="text-5xl font-medium tracking-tighter text-[#1F1F1F]">
			Have Question? <br /> We're Here to Help
		</h2>
		<p class="text-base tracking-tight text-gray-600">
			Find answers to frequently asked questions about us.
		</p>
	</section>

	<section class="mt-12 grid grid-cols-2 gap-5">
		<div class="flex flex-col gap-4">
			{#each questions_1 as question, idx}
				<div
					class={[
						' rounded-xl border px-3 py-4 ',
						question.isActive ? 'border-[#5953C3] bg-[#F8F9FF] ' : 'border-[#DDDDDD]'
					]}
				>
					<button class="flex justify-between w-full" onclick={() => handleAccordian('group_1', idx)}>
						<h3 class="text-base/4 font-medium text-[#1f1f1f]">{question.question}</h3>
						<span class={[" transition duration-300", question.isActive && "rotate-180"]}>{@render arrow_down(question.isActive)}</span>
					</button>

					{#if question.isActive}
						<p transition:slide class=" mt-2 text-sm/4 font-normal leading-snug text-[#23262E]">
							{question.answer}
						</p>
					{/if}
				</div>
			{/each}
		</div>

		<div class="flex flex-col gap-4">
			{#each questions_2 as question, idx}
				<div
					class={[
						' rounded-xl border px-3 py-4 ',
						question.isActive ? 'border-[#5953C3] bg-[#F8F9FF] ' : 'border-[#DDDDDD]'
					]}
				>
					<button class="flex justify-between w-full" onclick={() => handleAccordian('group_2', idx)}>
						<h3 class="text-base/4 font-medium text-[#1f1f1f]">{question.question}</h3>
						<span class={[" transition duration-300", question.isActive && "rotate-180"]}>{@render arrow_down(question.isActive)}</span>
					</button>

					{#if question.isActive}
						<p transition:slide class=" mt-2 text-sm/4 font-normal leading-snug text-[#23262E]">
							{question.answer}
						</p>
					{/if}
				</div>
			{/each}
		</div>
	</section>
</section>
