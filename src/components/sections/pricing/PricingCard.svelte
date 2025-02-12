<script lang="ts">
	let { category, header, benefit } = $props();
</script>

<section class="#border-[#EAE9FB] min-w-96 rounded-lg border-2 p-1">
	<div class="grid gap-6 bg-[#F6F7FF] p-3">
		<div class="inline-grid gap-4">
			<div
				class=" inline-flex w-fit gap-1 rounded-md bg-[#E8EBFF] px-[0.625rem] py-[6px] text-sm/[14px] font-medium tracking-tight text-[#2D43C9]"
			>
				{@render category()}
			</div>

			<div class="">{@render header()}</div>
		</div>

		<div class="grid gap-5">
			<div class="grid gap-3">{@render benefit()}</div>

			<button
				class=" w-full rounded border border-[#EAEAEA] bg-white py-3 text-base/4 font-medium tracking-tight text-[#1F1F1F] hover:bg-[#F1F1F1]"
				>Select Plan</button
			>
		</div>
	</div>
</section>
