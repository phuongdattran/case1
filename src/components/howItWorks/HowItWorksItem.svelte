<script>
  export let data;
  const { icon, alt, step, text } = data;
</script>

<div class="container">
  <div class="stepAndIconContainer">
    <div class="iconContainer">
      <img class="icon" src={icon} {alt} />
    </div>
    <p class="stepNumber">{step}</p>
  </div>
  <p class="text">{text}</p>
</div>

<style>
  .container {
    display: flex;
    flex: 1;
    flex-direction: column;
    align-items: center;
    position: relative;
    margin: 15px;
  }

  .stepAndIconContainer {
    height: 80px;
    margin-top: 15px;
  }

  .iconContainer {
    height: 80px;
  }

  .stepNumber {
    position: relative;
    bottom: 60px;
    left: -67px;
    color: #f29210;
    font-size: 60px;
    font-weight: 700;
    line-height: 23px;
    opacity: 0.28;
  }

  .text {
    font-size: 16px;
    line-height: 24px;
    text-align: center;
  }

  @media (max-width: 720px) {
    .container {
      display: grid;
      grid-template-columns: 1fr 4fr;
      align-items: center;
      gap: 15px;
    }

    .icon {
      height: 50%;
    }

    .stepNumber {
      bottom: 160px;
      left: -10px;
      font-size: 60px;
      font-weight: 700;
      line-height: 23px;
    }

    .text {
      text-align: left;
    }
  }

  @media (max-width: 1201px) {
    .stepNumber {
      left: -10px;
    }
  }
</style>
