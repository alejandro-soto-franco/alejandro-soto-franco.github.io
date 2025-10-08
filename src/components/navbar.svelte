<script>
    // TODO(@ale): read the svelte sveltekit documentation: https://svelte.dev/
    // i think you'll like it. it's used by all the fancy rust/haskell teams as their lean frontend framework of choice
</script>

<nav>
    <a href="#top">
        <span class="logo">A.S.F.</span>
    </a>
    <div>
        <a href='#math-physics'>
            <span class="link">Mathematical Physics</span>
        </a>
        <a href='#top'>
            <span class="link">Biomedical Engineering</span>
        </a>
        <a href='#contact-me'>
            <span class="button">Contact Me</span>
        </a>
    </div>
</nav>

<style>
    @font-face {
        font-family: 'lmmono';
        font-style: monospace;
        font-weight: 400;
        src: url('/fonts/lmmono12-regular.otf') format('otf');
    }

    @font-face {
        font-family: 'lmroman';
        font-style: normal;
        font-weight: 400;
        src: url('/fonts/lmmroman8-regular.otf') format('otf');
    }

    span.logo {
        font-family: lmmono;
    }

    span.link {
        font-family: lmroman;
        color: #9E1B34;
    }

    span.button {
        padding: 0.5rem 1rem;
        font-family: lmroman;
        background-color: #9E1B34;
        color: white;
        border-radius: 8px;
    }

    nav {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
    }

    div {
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: end;
    }
</style>
