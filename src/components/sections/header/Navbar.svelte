<script lang="ts">
	import { logo } from "@components/Logos.svelte";


</script>

<nav class="box-border px-24 flex items-center justify-between border-b border-[#F0F0F0]">
    <section class="flex items-center gap-16">
        <div>{@render logo()}</div>
        <ul class="flex items-center gap-10 text-base/4 font-medium text-[#3E3E3E] tracking-tight">
            <li class="py-6 border-y-2 border-transparent hover:border-b-[#5C43DC]"><a href="/">Overview</a></li>
            <li class="py-6 border-y-2 border-transparent hover:border-b-[#5C43DC]"><a href="/">Tools</a></li>
            <li class="py-6 border-y-2 border-transparent hover:border-b-[#5C43DC]"><a href="/">About Us</a></li>
            <li class="py-6 border-y-2 border-transparent hover:border-b-[#5C43DC]"><a href="/">Pricing</a></li>
            <li class="py-6 border-y-2 border-transparent hover:border-b-[#5C43DC]"><a href="/">Services</a></li>
        </ul>
    </section>

    <div>
        <button class="text-sm/[14px] font-semibold text-[#1F1F1F] border border-[#E9E9E9] rounded-md px-3 py-[10px]">Learn More</button>
        <button class="rounded-md px-3 py-[10px] text-sm/[14px] font-semibold bg-[#5254D3] text-white">Get Started</button>
    </div>
</nav>