<script lang="ts">
	import { facebook, instagram, linkedin, twitter } from "@components/Logos.svelte";

    let social_icons = $state([facebook, linkedin, instagram, twitter]);
</script>

<footer class="bg-[#020202] text-[#F0F0F0] px-12 ">
    <section class=" py-[4.5rem] grid grid-cols-2 gap-6 ">
        <div class="inline-grid gap-6">
            <h3 class=" text-[2.5rem]/[130%] font-medium tracking-tighter pr-12 ">Budget Saving, high flexibility and effectiveness. Start getting them now.</h3>
            <button class="rounded-md inline-flex w-fit px-4 py-[10px] text-sm/[14px] font-semibold bg-white text-[#020202]">Get Started</button>
        </div>

        <div class="flex justify-between">
            <div>
                <h4 class="text-base/4 font-medium tracking-tight mb-6">Navigation</h4>
                <ul class=" text-sm/[14px] font-light tracking-tight grid gap-4">
                    <li class=" hover:underline underline-offset-4 "><a href="/">Home</a></li>
                    <li class=" hover:underline underline-offset-4 "><a href="/">Tools</a></li>
                    <li class=" hover:underline underline-offset-4 "><a href="/">About Us</a></li>
                    <li class=" hover:underline underline-offset-4 "><a href="/">Pricing</a></li>
                    <li class=" hover:underline underline-offset-4 "><a href="/">Services</a></li>
                    <li class=" hover:underline underline-offset-4 "><a href="/">Contact Us</a></li>
                </ul>
            </div>

            <div>
                <h4 class="text-base/4 font-medium tracking-tight mb-6">Company</h4>
                <ul class=" text-sm/[14px] font-light tracking-tight grid gap-4">
                    <li class=" hover:underline underline-offset-4 "><a href="/">News</a></li>
                    <li class=" hover:underline underline-offset-4 "><a href="/">Career</a></li>
                    <li class=" hover:underline underline-offset-4 "><a href="/">Our Story</a></li>
                </ul>
            </div>

            <div>
                <h4 class="text-base/4 font-medium tracking-tight mb-6">Most Frequently Employed</h4>
                <ul class=" text-sm/[14px] font-light tracking-tight grid gap-4">
                    <li class=" hover:underline underline-offset-4 "><a href="/">Software Engineer</a></li>
                    <li class=" hover:underline underline-offset-4 "><a href="/">Graphic Designer</a></li>
                    <li class=" hover:underline underline-offset-4 "><a href="/">UI Design</a></li>
                    <li class=" hover:underline underline-offset-4 "><a href="/">UX Design</a></li>
                    <li class=" hover:underline underline-offset-4 "><a href="/">Web Programmer</a></li>
                </ul>
            </div>
        </div>
    </section>
    <section class=" py-9 flex justify-between items-center">
        <p class=" text-base/4 font-light tracking-tight ">©{new Date().getFullYear()} Remotin. All rights reserved. Developed by <a class=" text-white font-medium underline underline-offset-4 " href="https://mehedi-agency.vercel.app" target="_blank"><strong>Mehedi Hasan</strong></a>.</p>
        <div class="flex gap-4 items-center">
            {#each social_icons as social}
                <div>{@render social()}</div>
            {/each}
        </div>
    </section>
</footer>