<script>
    import { createEventDispatcher } from 'svelte'

    const dispatch = createEventDispatcher()

    const handleSayHello = (event) => {
        dispatch('sayhello', {
            text: 'Hola mundo'
        })
    }

</script>

<div>
    <button on:click={handleSayHello}>
        Say hello
    </button>
</div>

