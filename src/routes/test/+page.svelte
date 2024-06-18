<script>
    import {onMount} from "svelte"

    let canvas
    let ctx
    let isClient
    onMount(() => {
        console.log("mounted")
        isClient = true
        ctx = canvas.getContext("webgl")
        console.log(ctx)
    })
</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

<button>I AM A <s>SURGEON</s> BUTTON</button>

<input type="text" default="ligma" placeholder="ligma">

<canvas
    bind:this={canvas}
/> 