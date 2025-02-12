<script lang="ts">
    let { category, header, benefit } = $props();
</script>


<section class="border-2 #border-[#EAE9FB] rounded-lg p-1 min-w-96 ">
    <div class="p-3 bg-[#F6F7FF] grid gap-6">
        <div class="inline-grid gap-4">
            <div class=" w-fit inline-flex gap-1 tracking-tight text-[#2D43C9] rounded-md text-sm/[14px] font-medium py-[6px] px-[0.625rem] bg-[#E8EBFF] ">{@render category()}</div>

            <div class="">{@render header()}</div>
        </div>

        <div class="grid gap-5">
            <div class="grid gap-3">{@render benefit()}</div>

            <button class=" bg-white hover:bg-[#F1F1F1] border border-[#EAEAEA] rounded text-base/4 font-medium tracking-tight py-3 w-full text-[#1F1F1F] ">Select Plan</button>
        </div>
    </div>
</section>