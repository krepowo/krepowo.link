<script lang="ts">
   import Fa from "svelte-fa";
   import {
      faGithub,
      faInstagram,
      faTwitter,
      faDiscord,
   } from "@fortawesome/free-brands-svg-icons";
   import "@fortawesome/fontawesome-free/css/all.min.css";
   import Project from "./Project.svelte";
</script>

<div class="top">
   <div class="social">
      <a class="github" href="https://github.com/krepowo">
         <Fa icon={faGithub} size="2x" />
      </a>
      <a class="instagram" href="https://instagram.com/krepowo">
         <Fa icon={faInstagram} size="2x" />
      </a>
      <a class="twitter" href="https://twitter.com/krepowo">
         <Fa icon={faTwitter} size="2x" />
      </a>
      <a class="discord" href="https://discord.com/krepowo">
         <Fa icon={faDiscord} size="2x" />
      </a>
   </div>
   <div class="nav">
      <a class="btn-project" href="#home">Home</a>
      <a class="btn-project" href="#projects">Projects</a>
   </div>
</div>
