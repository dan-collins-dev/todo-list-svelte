<script>
    import PriorityPill from "./PriorityPill.svelte";
</script>

<article>
    <p class="name">Do the dirty Dishes</p>
    <p class="due-date">2010-10-10</p>
    <PriorityPill priority={"low"} />
</article>

<style>
    article {
        display: grid;
        grid-template-columns: 1fr 1fr;
        row-gap: 0.5rem;
    }

    .name {
    }

    .due-date {
        justify-self: end;
    }
</style>
