<script>
  export let data;
  const { icon, alt, text } = data;
</script>

<div class="container">
  <img class="icon" src={icon} {alt} />
  <p class="text">{@html text}</p>
</div>

<style>
  .container {
    display: grid;
    grid-template-columns: 1fr 6fr;
    gap: 30px;
    align-items: center;
    margin-bottom: 15px;
  }
</style>
