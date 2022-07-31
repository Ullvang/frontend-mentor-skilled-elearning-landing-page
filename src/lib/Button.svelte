<script>
    export let type;
    export let big = false;
</script>

<button class={type + (big ? " big" : "")}>
    Get Started
</button>

<style>
    button {
        border-radius: 100px;
        padding: 14px 32px;
        font-size: 18px;
        line-height: 28px;
        color: var(--white);
        border: none;
        font-weight: 700;
        /* letter-spacing: 1px; */
    }
    :global(.blue) {
        background-color: var(--dark-blue);
    }
    :global(.red) {
        background: linear-gradient(var(--orange), var(--pink-gradient));
    }
    :global(.purple) {
        background: linear-gradient(var(--blue-gradient), var(--pink-gradient));
    }
    .big {
        padding: 19px 32px 16px;
    }
    </style>