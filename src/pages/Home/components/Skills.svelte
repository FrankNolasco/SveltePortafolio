<script>
    import Card from "../../../components/molecules/Card.svelte";
</script>


<section class="skills-sections">

    <h3>My best skills </h3>


    <ul>
        <li>
            <Card hoverable>
                <img class="img-skill" src="https://www.alioze.com/wp-content/uploads/2016/11/react-js.png" alt="Developer React JS"/>
            </Card>
        </li>
        <li>
            <Card hoverable>
                <img class="img-skill" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSYR9gYh7t9TGdG1MEgCbKkqAEaciCt5sK7ZAOyCCdPjlp9rbvmu3D-Iu09g_zXrxuAKnY&usqp=CAU" alt="Developer React native"/>
            </Card>
        </li>
        <li>
            <Card hoverable>
                <img class="img-skill" src="https://miro.medium.com/max/365/1*Jr3NFSKTfQWRUyjblBSKeg.png" alt="Developer Node">
            </Card>
        </li>
        <li>
            <Card hoverable>
                <img class="img-skill" src="https://www.iperiusbackup.net/wp-content/uploads/2016/05/1768.sql_logo.png" alt="Developer SQL Server"/>
            </Card>
        </li>
        <li>
            <Card hoverable>
                <img class="img-skill" src="https://bluuweb.github.io/svelte-youtube/img/svelte.png" alt="Developer Svelte"/>
            </Card>
        </li>
    </ul>

</section>

<style>
    .skills-sections {
        align-items: center;
        flex-wrap: wrap;
        padding: 1em 5em;
        margin: 0;
        background-color: #f9f9f9;
    }

    ul {
        display: flex;
        justify-content: space-around;
        list-style: none;
        gap: 10px;
    }
    
    .img-skill {
        width: 150px;
        height: 50px;
        object-fit: contain;
    }

</style>
