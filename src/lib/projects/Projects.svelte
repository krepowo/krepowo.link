<script lang="ts">
   import Fa from "svelte-fa";
   import { faExternalLink } from "@fortawesome/free-solid-svg-icons";
</script>

<div class="projects">
   <h1 class="heading">List of my projects</h1>
   <div class="circle-zkr" />
   <div class="content zkr">
      <div class="project-info">
         <div class="info">
            <h1>ShortZKR</h1>
            <p>
               ShortZKR is a simple URL shortener. Created by me and ZKR team.
               It is also support custom alias. Go try it >:D
            </p>
         </div>
         <div class="icon">
            <img
               class="image"
               src="https://cdn.zkr.pw/pictures/webicon.jpg"
               alt="zkr icon"
            />
         </div>
      </div>
      <a class="visit" href="https://zkr.pw" target="_blank"
         >Visit <Fa icon={faExternalLink} size="1x" /></a
      >
   </div>
   <div class="circle-astatine" />
   <div class="content astatine">
      <div class="project-info">
         <div class="info">
            <h1>Astatine</h1>
            <p>
               An utility Discord Bot, built using <a
                  class="eris"
                  href="https://github.com/abalabahaha/eris"
                  target="_blank">Eris</a
               > library. Have many cool features and commands. This bot is now abondoned
               but still online and usable 👍
            </p>
         </div>
         <div class="icon">
            <img class="image" src="./astatine-logo.png" alt="astatine logo" />
         </div>
      </div>
      <a class="visit" href="#projects"
         >Invite <Fa icon={faExternalLink} size="1x" /></a
      >
   </div>
</div>
