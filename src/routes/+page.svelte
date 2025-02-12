<script lang="ts">
	import Faq from '@components/sections/faq/Faq.svelte';
	import Footer from '@components/sections/footer/Footer.svelte';
	import Header from '@components/sections/header/Header.svelte';
	import Howitwork from '@components/sections/how_it_work/Howitwork.svelte';
	import Icp from '@components/sections/icp/Icp.svelte';
	import Pricing from '@components/sections/pricing/Pricing.svelte';
	import Solution from '@components/sections/solution/Solution.svelte';
</script>

<Header />
<main>
	<Icp />
	<Solution />
	<Howitwork />
	<Pricing />
	<Faq />
</main>
<Footer />

<svelte:head>
	<title>Remotin - Remote Worker Service Provider</title>
</svelte:head>
