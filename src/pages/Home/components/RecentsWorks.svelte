<script>
import Button from "../../../components/atoms/Button.svelte";


import Card from "../../../components/molecules/Card.svelte";

</script>
<div class="section-recents-works">
    <div class="left-w">
        <h3>Recent Works</h3>
        <span>works got most attention</span>
        <p>
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Beatae modi molestias perferendis dolorum. Quia voluptatibus nulla et sunt, culpa tempora, obcaecati autem voluptates modi tempore ut doloremque ducimus dolorum illum.
        </p>
        <Button label="View all Works" variant="link" size="medium"/>
    </div>
    <div class="projects-recents">
        <Card elevation>
            <h4>Web Solutions</h4>
            <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                Pellentesque euismod, urna eu tincidunt consectetur,
                nisi nisl aliquam nunc, eget consectetur nunc nisl eu
                ligula.
            </p>
        </Card>
        <Card elevation>
            <h4>Web Solutions</h4>
            <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                Pellentesque euismod, urna eu tincidunt consectetur,
                nisi nisl aliquam nunc, eget consectetur nunc nisl eu
                ligula.
            </p>
        </Card>
    </div>


    
        

</div>


<style>
    .section-recents-works {
        display: flex;
        padding: 1em 5em;

    }

    .left-w {
        width: 50%;
    }
    .projects-recents {
        display: flex;
        justify-content: space-around;
        align-items: center;
        width: 100%;
        gap: 10px
    }
</style>