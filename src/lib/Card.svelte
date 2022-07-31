<script>
    export let title;
    export let text;
    export let icon;
</script>

<div>
    <img src="/assets/{icon}.svg" alt={icon}/>
    <h3>{title}</h3>
    <p>{text}</p>
    <button>
        Get Started
    </button>
</div>

<style>
    div {
        background-color: var(--white);
        padding: 64px 32px 40px;
        border-radius: 15px;
        position: relative;
        margin-top: 24px;
        min-height: 322px;
    }
    button {
        color: var(--pink);
        border: none;
        background-color: var(--white);
        padding: 0px;
        font-weight: 700;
        font-size: 18px;
        line-height: 28px;
        /* letter-spacing: 1px; */
        position: absolute;
        bottom: 40px;
    }
    p {
        margin: 24px 0px;
        /* font-weight: 500; */
        /* letter-spacing: 0; */
    }
    img {
        position: absolute;
        top: -24px;
    }
</style>