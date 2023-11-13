<script lang="ts">
    import Fa from "svelte-fa";
    import { faExternalLink } from "@fortawesome/free-solid-svg-icons";

    const projects = [
        {
            name: "ShortZKR",
            button: [
                {
                    text: "Visit",
                    url: "https://zkr.pw",
                },
                {
                    text: "Invite Bot",
                    url: "https://zkr.pw/bot",
                },
            ],
            image: "./webicon.webp",
            description: `ShortZKR is a simple URL shortener. Created by me and ZKR team. It is also support custom alias and have an official Discord Bot. Go try it >:D`,
        },
        {
            name: "Astatine",
            link: "https://astatine.pw",
            button: [
                {
                    text: "Invite Bot",
                    url: "https://discord.com/api/oauth2/authorize?client_id=865838415517188106&permissions=274878228544&scope=bot%20applications.commands",
                },
            ],
            image: "./astatine-logo.webp",
            description: `A utility Discord Bot, created using Eris library. Have many cool features and commands. This bot is now abandoned but still online and usable 👍`,
        },
        {
            name: "TextBin",
            link: "https://textbin.link",
            button: [
                {
                    text: "Visit",
                    url: "https://textbin.link",
                },
            ],
            image: "./textbin.webp",
            description: `Text paste service like PasteBin but with many language syntax support and VSCode like text editor. Created using Next.js and tailwindcss`,
        },
        {
            name: "OwO Freeroam",
            link: "samp://gta.krepowo.link:25611",
            button: [
                {
                    text: "Play",
                    url: "samp://gta.krepowo.link:25611",
                },
            ],
            image: "./owofr.webp",
            description: `A GTA San Andreas Multiplayer server. OwO Freeroam is a freeroam server, which mean you can do anything you want in this server. Yes, anything.`,
        },
    ];
</script>

<div class="projects">
    <h1 class="heading">List of my projects</h1>
    {#each projects as project}
        <div class={`circle-${project.name.toLowerCase().replace(" ", "_")}`} />
        <div class={`content ${project.name.toLowerCase()}`}>
            <div class="project-info">
                <div class="info">
                    <h1>{project.name}</h1>
                    <p>{project.description}</p>
                </div>
                <div class="icon">
                    <img
                        class="image"
                        src={project.image}
                        alt={`${project.name} icon`}
                    />
                </div>
            </div>
            {#each project.button as button}
                <a class="visit" href={button.url} target="_blank">
                    {button.text}
                    <Fa icon={faExternalLink} size="1x" />
                </a>
            {/each}
        </div>
    {/each}
</div>
