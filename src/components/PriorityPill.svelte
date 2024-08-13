<script>
    export let priority = "";
    let colorClass;

    const addColorClass = () => {
        if (priority === "low") {
            colorClass = "low";
        } else if (priority === "med") {
            colorClass = "med";
        } else {
            colorClass = "high";
        }

        return colorClass;
    };

    const formatPriority = () => {
        return priority.slice(0, 1).toLocaleUpperCase() + priority.slice(1);
    };
</script>

<div class={addColorClass()}>
    <p>{formatPriority()}</p>
</div>

<style>
    div {
        display: flex;
        background-color: white;
        padding: 0.25rem;
        width: 5rem;
        justify-content: center;
        border-radius: 1rem;
        grid-column: 2;
        justify-self: end;
        margin-top: 0.5rem;
    }

    p {
    }

    .low {
        background-color: rgb(111, 111, 221);
    }

    .med {
        background-color: rgb(247, 176, 52);
    }

    .high {
        background-color: rgb(250, 115, 115);
    }
</style>
