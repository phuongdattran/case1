<script>
  import { howItWorksContent } from "../../data";
  import TitleBar from "../TitleBar.svelte";
  import HowItWorksItem from "./HowItWorksItem.svelte";
</script>

<section class="container">
  <div id="titleContainer">
    <TitleBar />
    <h3>Et, concrètement, comment ça marche ?</h3>
  </div>
  <div id="itemsContainer">
    {#each howItWorksContent as data (data.step)}
      <HowItWorksItem {data} />
    {/each}
  </div>
</section>

<style>
  .container {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 150px;
    margin-bottom: 50px;
  }

  #titleContainer {
    max-width: 300px;
    text-align: center;
  }

  #itemsContainer {
    display: flex;
    flex-direction: row;
  }

  h3 {
    text-align: center;
    margin: 25px auto;
  }

  @media (max-width: 1201px) {
    .container {
      margin-top: 100px;
    }

    #titleContainer {
      margin-bottom: 30px;
    }

    #itemsContainer {
      display: block;
    }

    h3 {
      margin: 0 auto;
      width: 80%;
    }
  }
</style>
