<script>
  import Navbar from "./components/Navbar.svelte";
  import Hero from "./components/Hero.svelte";
  import Projects from "./components/Projects.svelte";
</script>
<div class="app">
<div class="navbar"><Navbar /></div>
<Hero />
<div id="projects"><Projects /></div>

</div>
<style>
  .navbar {
    display: flex;
    justify-content: center;
    margin-top: 0;
  }
  .app {
  width: inherit;
  }

</style>