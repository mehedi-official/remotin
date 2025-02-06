<script lang="ts">
    let { category, header, benefit } = $props();
</script>


<section>
    <div>{@render category()}</div>

    <div>{@render header()}</div>

    <div>{@render benefit()}</div>

    <button>Select Plan</button>
</section>