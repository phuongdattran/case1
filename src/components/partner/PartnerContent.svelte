<script>
  import { partnerContent } from "../../data";
  import TitleBar from "../TitleBar.svelte";
  import PartnerItem from "./PartnerItem.svelte";
</script>

<section class="container">
  <div id="titleContainer">
    <TitleBar />
    <h3>Decathlon Partner</h3>
    <p id="titleDescription">C’est quoi?</p>
  </div>
  <div>
    {#each partnerContent as data (data.id)}
      <PartnerItem {data} />
    {/each}
  </div>
</section>

<style>
  .container {
    display: grid;
    grid-template-columns: 1fr 2fr;
    gap: 20px;
    align-items: center;
  }

  #titleDescription {
    font-family: "Roboto Condensed", sans-serif;
    font-weight: 400;
    font-size: 20px;
    line-height: 24px;
  }

  @media (max-width: 720px) {
    .container {
      display: block;
      margin-top: -20px;
    }

    #titleContainer {
      display: flex;
      flex-direction: column;
      align-items: center;
    }

    #titleDescription {
      margin-top: 0;
    }

    h3 {
      margin-bottom: 10px;
    }
  }
</style>
