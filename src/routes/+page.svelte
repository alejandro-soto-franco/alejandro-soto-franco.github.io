<script>
    // Before all else, make sure you have node installed, and run npm install

    import { Math } from 'svelte-math';
    // TODO(@ale): you should be able to insert latex in the future using this package above.
    // Check out the docs at https://www.npmjs.com/package/svelte-math and especially Usage > With Props

    import Navbar from '../components/navbar.svelte';
    import torus from '$lib/assets/torus.gif'; // TODO(@ale): put your torus gif animation in lib/assets

    // TODO(@ale): i believe you should be able to just run "npm deploy" to publish to github pages
    // if it doesn't work, try debugging my "deploy" script in package.json
</script>

<Navbar />
<main>
    <h1 id="top">Alejandro Soto Franco M.Sci.Eng.</h1>
    <h2>Nonlinear dynamical systems researcher</h2>
    <div class="image-spread">
        <img alt="genus-6 torus" src={torus} />
        <span class="caption">genus-6 torus</span>
        <span class="credit">credit: C. Zhu</span>
    </div>
    <h2>Follow the <span class="red">red links</span>. BME under construction.</h2>
    <hr id="math-physics" />
    <h1>Mathematical physics</h1>
    <p>I study the mathematical structures underlying dynamics, geometry, and topology of complex physical systems</p>
    <h2>Spring 2025: Active k-atic fluids on Riemannian 2-manifolds</h2>
    <ul>
        <li><a href="/">29 April group meeting notes, Dan Beller Group</a></li>
        <li><a href="/">17 April super-group meeting slides, “Topological defect dynamics in active nematic fluids on Riemannian 2-manifolds”, JHU P&A Soft Matter</a></li>
    </ul>
    <h2>Fall 2024: Beris-Edwards nemato-hydrodynamics simulation of +1/2 defect braiding on epicycloid domains</h2>
    <ul>
        <li><a href="/">Preprint with Brandon Klein</a>(status: submitted to PRX, hooray!)</li>
        <li><a href="/">Cardioid-confined golden braiding videos</a></li>
        <li><a href="/">Nephroid-confined silver braiding videos</a></li>
    </ul>
    <hr id="contact-me" />
    <h1>Contact Me</h1>
    <p>
        Physics/math-related queries: sotofranco.math@gmail.com<br />
        Engineering queries: sotofranco.eng@gmail.com<br />
        JHU student email: asoto12@jhu.edu<br />
        Friends and family: alejandro.jsfr@gmail.com
    </p>
</main>

<style>
    /* TODO(@ale): modify otf file imports to use the ones you want to use from static/fonts */

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

    main {
        display: flex;
        flex-direction: column;
        gap: 1rem;
    }

    div.image-spread {
        width: 100%;
        height: fit-content;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: start;
        gap: 1rem;
    }

    span.caption {
        font-family: lmroman;
        font-size: 0.8rem;
    }

    span.credit {
        font-family: lmroman;
        font-size: 0.5rem;
    }

    span.red {
        color: #9E1B34;
    }

    h1 {
        font-family: lmroman;
    }

    h2 {
        font-family: lmroman;
    }

    p {
        font-family: lmroman;
    }

    a {
        color: #9E1B34;
    }

</style>
