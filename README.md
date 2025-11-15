# ShuttleAI Projects Showcase  

**Automatically discover and announce new public GitHub projects that use the [ShuttleAI API](https://api.shuttleai.com).**  

Every 6 hours a GitHub Action scans for **public, non-fork** repositories that have the topic **`shuttleai`**.  

When new ones appear, a nicely formatted embed is posted as a **new thread** in the [**#projects**](https://discord.com/channels/1152262611291869237/1434724773765845033) forum channel of the ShuttleAI Discord.

---

## How to Get Featured  

1. **Make your repo public**  

2. **Add the topic** `shuttleai`  

   - Go to **Settings → Topics** → type `shuttleai` → **Add**  

3. **Use the ShuttleAI API** somewhere in the code (any endpoint, any language)  

4. Push a commit – the next run (max 6 h) will pick it up!  

> **Tip:** Mention the API in your README or a comment so it’s obvious the project is powered by ShuttleAI.

---

## What the Discord post looks like  

```

New ShuttleAI-powered projects just dropped! Check them out and show some love

[Embed: Latest Projects on GitHub]

- **my-cool-bot** by @johndoe

  https://github.com/johndoe/my−cool-bot

  A Discord bot that generates memes with ShuttleAI image models

[Footer: Add `shuttleai` topic to your repo to be featured! → https://github.com/topics/shuttleai]

```

---

## For Developers

The showcase is powered by a **GitHub Actions workflow** (`.github/workflows/showcase.yml`).  

It:

* Queries GitHub Search API (`topic:shuttleai+fork:false`)  

* Keeps a `seen_repos.json` file to avoid duplicates  

* Sends a webhook payload to Discord (creates a thread)  

Feel free to fork or study the workflow if you want similar automation elsewhere.

---

## Questions?

Create a thread in our [**#support**](https://discord.com/channels/1152262611291869237/1210395499526627448) channel in our Discord.

---

*Maintained by the ShuttleAI team • Last updated November 2025*

https://shuttleai.com | https://discord.gg/shuttleai
