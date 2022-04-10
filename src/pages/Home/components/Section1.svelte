<script>
  import Button from "../../../components/atoms/Button.svelte";
</script>

<section class="section-1">
  <div class="information-relevant">
    <h1>Frank Nolasco Velasquez</h1>
    <h3>Web developer</h3>
    <p>
      Lorem ipsum dolor sit amet consectetur, adipisicing elit. Cumque sint vel
      dolor eaque fugit voluptatem ducimus praesentium iusto laudantium placeat
      nihil est, incidunt assumenda perspiciatis. Voluptatum eveniet quia
      veniam? Sequi.
    </p>
    <div class="buttons-display">
      <Button><i class="fa fa-file-pdf"/> CV PDF</Button>
      <Button variant="github"><i class="fab fa-github"/> GitHub</Button> 
    </div>

  </div>
  <img
    class="kakashi"
    src="https://www.pngplay.com/wp-content/uploads/12/Kakashi-Wallpaper-Transparent-Background.png"
    alt="Kakashi Hatake - 6to Hokage"
  />
</section>

<style>
  .section-1 {
    box-sizing: border-box;
    padding: 0 60px;
    background-color: #f0f0f0;
    display: flex;
    justify-content: space-around;
  }

  .buttons-display {
    display: flex;
    gap: 1em;
  }

  .information-relevant {
    align-self: center;
    padding: 1em 5em;
  }

  .information-relevant > h1 {
    font-size: 2.5em;
    font-weight: 900;
    margin: 0;
  }

  .kakashi {
    width: 400px;
  }
</style>
