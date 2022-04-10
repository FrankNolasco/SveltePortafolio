<script>
    export let size = "big"
    export let variant = "primary"
</script>

<button class={`button ${variant} ${size}`}>
    <span>
        <slot></slot>
    </span>
</button>

<style>

    .button {
        border: none;
        cursor: pointer;
    }

    .big {
        padding: .6em 1.5em;
        border-radius: .5em;
        font-size: 1.2em;
    }


    .medium {
        padding: .4em 1em;
        border-radius: .25em;
        font-size: 1em;
    }

    .small {
        padding: .2em .5em;
        border-radius: .125em;
        font-size: .8em;
    }

    .primary { 
        background-color: rgb(255, 165, 62);
        color: white;
        /* bordex shadow  */
        box-shadow: 2px 2px 5px rgba(194, 182, 182, 0.875);
    }

    .github { 
        /* border: solid 1px rgb(193, 184, 184); */
        color: rgb(61, 61, 61);
        box-shadow: 2px 2px 5px rgba(194, 182, 182, 0.875);
    }



    .link {
        color: rgb(255, 165, 62);
        background-color: transparent;
    }


</style>