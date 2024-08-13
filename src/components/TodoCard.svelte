<script>
    import ActionButtons from "./ActionButtons.svelte";
    import TodoInfo from "./TodoInfo.svelte";
</script>

<article>
    <TodoInfo />
    <ActionButtons />
</article>

<style>
    article {
        background-color: rgb(194, 190, 237);
        display: flex;
        flex-direction: column;
        border: none;
        border-radius: 0.25rem;
        margin: 1rem 0.5rem;
        padding: 0.5rem;
        gap: 1rem;
    }
</style>
