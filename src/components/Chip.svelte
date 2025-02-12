<script lang="ts">
	import { logo_icon } from "./Icons.svelte";
    let { children } = $props();
</script>

{#if children}
    <div class="inline-flex gap-2 items-center w-fit py-[6px] px-2 border border-[#EEEDF0] rounded-md text-[#1F1F1F] text-sm/[14px] font-normal ">
        {@render logo_icon()}
        {@render children()}
    </div>
{/if}

