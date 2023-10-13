<script>
  import Navbar from "./lib/Navbar.svelte";
  import Header from "./lib/Header.svelte";
  import Projects from "./lib/Projects.svelte";
  import { Router, Route } from "svelte-routing";
    import Contact from "./lib/Contact.svelte";
  export let url = "";
</script>

<Router {url}>
  <header>
    <Navbar />
  </header>
  <main>
    <Route path="/"><Header /></Route>
    <Route path="/projects" component={Projects} />
  </main>
  <Contact/>
</Router>

<style>
  main {
    margin-top: 3.5rem;
    margin-inline: 10rem;
  }

  @media (max-width: 745px) {
    main {
      padding-inline: 3rem;
    }
  }
</style>
