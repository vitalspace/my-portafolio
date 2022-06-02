<script>
  import "./css/app.css";
  import { Router, Route, Link } from "svelte-navigator";

  import Bio from "./bio.svelte";
  import Menu from "./menu.svelte";
  import Contact from "./contact.svelte";
  import Index from "./index.svelte";
</script>

<Router>
  <header>
    <nav>
      <Menu/>
      <!-- <Link to="/">Home</Link> -->
      <!-- <Link to="bio">Bio</Link> -->
      <!-- <Link to="contact">Contact</Link> -->
    </nav>
  </header>

  <main>
    <Route path="/">
      <Index />
    </Route>

    <Route path="bio">
      <Bio />
    </Route>

    <Route path="contact">
      <Contact />
    </Route>
  </main>
</Router>
