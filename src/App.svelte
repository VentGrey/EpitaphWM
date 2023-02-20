<script lang="ts">
  /* Assets Import */
  import logo from "./assets/icon.png";
  import Features from "./components/Features.svelte";
  import Music from "./components/Music.svelte";
  import GoToTop from "./components/GoToTop.svelte";

  /* Components import */
  import Hero from "./components/Hero.svelte";
  import Footer from "./Footer.svelte";
  import Contributors from "./components/Contributors.svelte";
</script>

<style>
  .navbar-epitaph {
    backdrop-filter: blur(30px);
  }
</style>

<!-- Place the Navbar here -->
<header class="d-flex flex-wrap justify-content-center py-3 mb-4 sticky-top navbar-epitaph shadow">
      <a href="/" class="d-flex align-items-center mb-3 mb-md-0 me-md-auto text-dark text-decoration-none">
        <img height="64" width="64" class="img-fluid mx-2" src="{logo}" alt="Epitaph logo">
        <span class="fw-light fs-1 text-red">E</span>
        <span class="fw-light fs-1 text-peach">P</span>
        <span class="fw-light fs-1 text-yellow">I</span>
        <span class="fw-light fs-1 text-green">T</span>
        <span class="fw-light fs-1 text-blue">A</span>
        <span class="fw-light fs-1 text-purple">P</span>
        <span class="fw-light fs-1 text-light">H</span>
      </a>

      <ul class="nav nav-pills">
        <li class="nav-item"><a rel="noreferrer" target="_blank" href="https://youtu.be/vXrpFxHfppI?t=372" class="nav-link text-light text-decoration-none border mx-2" aria-current="page">Why Epitaph?</a></li>
        <li class="nav-item"><a rel="noreferrer" target="_blank" href="https://github.com/VentGrey/Epitaph/wiki" class="nav-link text-light text-decoration-none border mx-2">Install</a></li>
        <li class="nav-item"><a href="#music" class="nav-link text-decoration-none text-light border mx-2">Support music!</a></li>
      </ul>
</header>


<!-- Place the main content here -->
<Hero/>
<Features/>
<Music/>
<Contributors/>

<!-- Place the Go to top button here -->
<GoToTop/>

<!-- Always show footer-->
<Footer/>