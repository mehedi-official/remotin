<script lang="ts">

	import PricingCard from "./PricingCard.svelte";

</script>


<section>
    <section>
        <div>
            <h2>Pricing</h2>
        </div>

        <h2>Plans that fit your needs, pricing that's fair.</h2>
        <p>Pay only for what you need, with transparent pricing and no hidden fees.</p>
    </section>

    <section>
        <PricingCard>
            {#snippet category()}
                <span>Starter Plan</span>
            {/snippet}

            {#snippet header()}
                <div>
                    <h3>$6,000 <span>/month</span></h3>
                    <p>Perfect for small teams.</p>
                </div>
            {/snippet}

            {#snippet benefit()}
                <p>Default Analytics dashboard</p>
            {/snippet}
        </PricingCard>
    </section>
</section>