<script lang="ts">
	import Footer from "@components/sections/footer/Footer.svelte";
	import Header from "@components/sections/header/Header.svelte";
	import Howitwork from "@components/sections/how_it_work/Howitwork.svelte";
	import Icp from "@components/sections/icp/Icp.svelte";
	import Pricing from "@components/sections/pricing/Pricing.svelte";

</script>

<Header />
<main>
    <Icp />
	<Howitwork />
	<Pricing />
</main>
<Footer />

<svelte:head>
	<title>Remotin - Remote Worker Service Provider</title>
</svelte:head>