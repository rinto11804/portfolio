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
    display: flex;
    width: 100%;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }
</style>
