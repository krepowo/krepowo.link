<script lang="ts">
    import Fa from "svelte-fa";
    import { faExternalLink } from "@fortawesome/free-solid-svg-icons";

    const projects = [
        {
            name: "ShortZKR",
            button: [
                {
                    text: "Visit",
                    url: "https://zkr-front.vercel.app/",
                },
                {
                    text: "Invite Bot",
                    url: "https://zkr-front.vercel.app/",
                },
            ],
            image: "./webicon.webp",
            description: `ShortZKR is a simple URL shortener. Created by me and ZKR team. It is also support custom alias and have an official Discord Bot. Go try it >:D. Our old domain is 'zkr.pw' but it's expired.`,
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
                    url: "https://textbin.vercel.app/",
                },
            ],
            image: "./textbin.webp",
            description: `Text paste service like PasteBin but with many language syntax support and VSCode like text editor. Created using Next.js and tailwindcss`,
        },
        {
            name: "Network Utils",
            link: "https://discord.com/oauth2/authorize?client_id=936446020441755708&permissions=296960&integration_type=0&scope=applications.commands+bot",
            button: [
                {
                    text: "Invite Bot",
                    url: "https://discord.com/oauth2/authorize?client_id=936446020441755708&permissions=296960&integration_type=0&scope=applications.commands+bot",
                }
            ],
            image: "./network-utils.webp",
            description: "Network Utils is a Discord bot that allows you to get information about internet stuff, for like DNS lookup, domain WHOIS, and more. Created using Discord.js Library"
        },
        {
            name: "osu2Discord",
            link: "https://github.com/krepowo/osu2discord",
            button: [
                {
                    text: "Github",
                    url: "https://github.com/krepowo/osu2discord",
                },
            ],
            image: "./osu.webp",
            description: "Send osu! in-game chat to a Discord channel using webhook."
        }
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
