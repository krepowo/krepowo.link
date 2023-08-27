<script lang="ts">
   import Fa from "svelte-fa";
   import {
      faGithub,
      faInstagram,
      faTwitter,
      faDiscord,
      faYoutube,
   } from "@fortawesome/free-brands-svg-icons";
   import "@fortawesome/fontawesome-free/css/all.min.css";
</script>

<div class="top">
   <div class="social">
      <a
         class="github"
         href="https://github.com/krepowo"
         aria-label="krepowo github"
         target="_blank"
      >
         <Fa icon={faGithub} size="2x" />
      </a>
      <a
         class="instagram"
         href="https://instagram.com/krepowo"
         aria-label="krepowo instagram"
         target="_blank"
      >
         <Fa icon={faInstagram} size="2x" />
      </a>
      <a
         class="twitter"
         href="https://twitter.com/Qwerty_Krep"
         aria-label="krepowo twitter"
         target="_blank"
      >
         <Fa icon={faTwitter} size="2x" />
      </a>
      <a
         class="discord"
         href="https://discord.com/users/620393180168323082"
         aria-label="krepowo discord"
         target="_blank"
      >
         <Fa icon={faDiscord} size="2x" />
      </a>
      <a
         class="youtube"
         href="https://youtube.com/@krepowo"
         target="_blank"
         aria-label="krepowo youtube"
      >
         <Fa icon={faYoutube} size="2x" />
      </a>
   </div>
   <div class="nav">
      <a class="btn-project" href="#home">Home</a>
      <a class="btn-project" href="#projects">Projects</a>
   </div>
</div>
