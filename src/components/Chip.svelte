<script lang="ts">
	import { logo_icon } from './Icons.svelte';
	let { children } = $props();
</script>

{#if children}
	<div
		class="inline-flex w-fit items-center gap-2 rounded-md border border-[#EEEDF0] px-2 py-1 text-sm/[14px] font-normal text-[#1F1F1F]"
	>
		{@render logo_icon()}
		{@render children()}
	</div>
{/if}
