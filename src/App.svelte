<script>
  import Navbar from "./components/Navbar.svelte";
  import Hero from "./components/Hero.svelte";
  import Projects from "./components/Projects.svelte";
  import About from "./components/About.svelte";
  import Tech from "./components/Tech.svelte";
</script>
<div class="app">
<div class="navbar"><Navbar /></div>
<Hero />
<About />
<Tech />
<div id="projects"><Projects /></div>

</div>
<style>
  .navbar {
    /* display: flex;
    justify-content: center;
    margin-top: 0; */
    position: fixed;
    top: 20px;
    left: 50%;
    transform: translate(-50%, 0%);
    z-index: 1;
  }
  .app {
  width: inherit;
  }

</style>