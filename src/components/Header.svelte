<script>
  import { headerContent } from "../data";
</script>

<header>
  <div class="container">
    <h1>{headerContent.title}</h1>
    <h2>{headerContent.description}</h2>
  </div>
  <div id="skew" />
</header>

<style>
  header {
    position: relative;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 600px;
    max-width: 100%;
    background-repeat: no-repeat;
    background-size: auto 320%;
    background-position: bottom -427px right -710px;
    background-image: url("https://contents.mediadecathlon.com/p1896013/k$ef392655b294171ec3ac508acdd82efa/QUECHUA%20ATHMOSPHERE%20%20%20SOCIAL%20MEDIA%20%20NEWSLETTER%20%20ADVICES.jpg?f=2000x2000");
    background-color: #0082c3;
    overflow: hidden;
  }

  h2 {
    margin-left: 20%;
    margin-right: 20%;
  }

  .container {
    position: relative;
    bottom: 20px;
  }

  #skew {
    position: absolute;
    height: 180px;
    bottom: -90px;
    right: 0;
    left: 0;
    background-color: #fff;
    -webkit-transform: skewY(-5deg);
    -moz-transform: skewY(-5deg);
    -o-transform: skewY(-5deg);
    -ms-transform: skewY(-5deg);
    transform: skewY(-5deg);
  }

  @media (max-width: 720px) {
    h1 {
      margin-top: 20px;
      margin-bottom: 30px;
    }

    h2 {
      margin-left: 5%;
      margin-right: 5%;
    }

    header {
      height: 340px;
      background-size: auto 120%;
      background-position: bottom 60px center;
    }
  }
</style>
