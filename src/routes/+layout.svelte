<script>
    import picio from "@picocss/pico"
</script>

<nav class="layout"> 
    <a prefetch href="/">Home</a>
</nav>
<main>
    <slot />
</main>

<footer>
    Pateogroup Incorporated 2022
</footer>

<style>
    nav {
        background: rgba(0,0,0,0.4);
        padding-top: 1rem;
        padding-bottom: 1rem;
    }

    nav, footer {
        text-transform: uppercase;
        font-size: 0.7rem;
        letter-spacing: 0.2px;
        font-weight: 500;
    }

    footer {
        text-align: center;
        margin: 3rem 0;
        color: rgb(255,255,255, 0.4);
    }

    :global(html) {
        background: rgb(20,20,40);
        overflow-y: scroll;
    }
    :global(.layout) {
        --width: 700px;
        padding-left: max(1rem, calc(calc(100vw - var(--width)) /2));
        padding-right: max(1rem, calc(calc(100vw - var(--width)) /2));
    }

    main {
        margin-bottom: 5rem;
        margin-top: 5vw;
    }
</style>