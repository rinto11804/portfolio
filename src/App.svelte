<script>
  import Navbar from "./lib/Navbar.svelte";
  import Header from "./lib/Header.svelte";
</script>

<Navbar />
<main>
  <Header />
</main>

<style>
  main {
    width: 100%;
    padding-inline: 20rem;
  }

  @media (max-width: 745px) {
    main {
      padding-inline: 3rem;
    }
  }
</style>
