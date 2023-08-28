<script lang="ts">
   import Center from "./lib/info/Center.svelte";
   import Projects from "./lib/projects/Projects.svelte";
   import Social from "./lib/info/Top.svelte";
   import Scroll from "./lib/info/Scroll.svelte";
   import Footer from "./lib/footer/Footer.svelte";
</script>

<main>
   <div id="home">
      <Social />
      <Center />
      <Scroll />
   </div>
   <div class="line" />
   <div id="projects">
      <Projects />
   </div>
   <div class="line" />
   <div class="footer">
      <Footer />
   </div>
</main>
