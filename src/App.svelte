<script>
  import { Router, Route } from "svelte-routing";
  import Home from "./routes/home/Home.svelte";
  import AboutEestec from "./routes/about/eestec/AboutEestec.svelte";
  import AboutXanthi from "./routes/about/xanthi/AboutXanthi.svelte";

  export let url = "/";
</script>

<Router {url}>
  <nav>
    <a href="/"><img alt="EESTEC LOGO" /></a>
    <a href="/"><img alt="" /></a>
    <a href="/about">About Us</a>
    <a href="/events">Events</a>
    <a href="/sponsors">Sponsors</a>
    <a href="/contact">Contact Us</a>
    <a href="/blog">GR/EN</a>
  </nav>
  <div>
    <!-- <Route path="/sponsors" component={BlogPost} /> -->
    <Route path="/about/eestec"><AboutEestec /></Route>
    <Route path="/about/xanthis"><AboutXanthi /></Route>
    <Route path=""><Home /></Route>
  </div>
</Router>

<style>
  nav {
    display: flex;
  }
  img {
    flex: 1;
  }
  a {
    font-size: xx-large;
    padding: 25px;
    flex: 1;
    font: Roboto;
    color: #990008;
    text-decoration: none;
    text-decoration-line: none;
  }
</style>
