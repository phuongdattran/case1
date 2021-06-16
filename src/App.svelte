<script>
  import Header from './components/Header.svelte'
  import PartnerContent from './components/partner/PartnerContent.svelte'
  import HowItWorksContent from './components/howItWorks/HowItWorksContent.svelte'
</script>

<Header />
<main>
  <PartnerContent />
  <HowItWorksContent />
</main>

<style>
  main {
    position: relative;
    margin: 0 17%;
  }

  @media (max-width: 720px) {
    main {
      margin: 0 7%;
    }
  }
</style>
