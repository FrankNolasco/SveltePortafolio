<script> 
    export let elevation = false
    export let hoverable = false

</script>

<div class={`card ${elevation && "elevation"} ${hoverable && "hoverable"}`}>
    <slot></slot>
</div>


<style>
    .card {
        padding: 1em;
        border-radius: .25em;
        background: white;
    }

    .elevation {
        box-shadow: 2px 2px 5px rgba(234, 225, 225, 0.875);
    }

    .hoverable{ 
        transition: box-shadow .8s;
    }


    .hoverable:hover{
        box-shadow: 2px 2px 5px rgba(234, 225, 225, 0.875);
    }
</style>

