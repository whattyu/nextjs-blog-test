---
title: "Discord Experiments"
date: 2022/4/27
description: "how to try discord experiments"
tag: How to
author: Whattyu
---

> ⚠️ It's breaking TOS so be carefully

If you want to try things that discord does that are not yet published you need to do a few things. In this post we'll show how to unblock the "Experiment" tab and how to download the development version of Discord (no canary but you can use canary).

# Download development version of Discord
When we want to try the latest unreleased stuff, we need a different client than Canary. These things come to canary later.
You need to download Discord Development. Just open this link:

> https://discordapp.com/api/download/development?platform=win (Windows)

> https://discordapp.com/api/download/development?platform=linux&format=deb (Linux, deb)

> https://discordapp.com/api/download/development?platform=linux&format=tar.gz (Linux, tar.gz)

> https://discordapp.com/api/download/development?platform=osx (Mac)

# Open console, use script
If we already have Discord Development downloaded, all we need to do is open the console in the client using the shortcut CTRL + SHIFT + I and then paste this code into the console:
```JavaScript
Object.defineProperty(
  (webpackChunkdiscord_app.push([[""], {}, (e) => {
    m = [];
    for (let c in e.c) m.push(e.c[c]);
  }]),
    m).find((m) => m?.exports?.default?.isDeveloper !== void 0).exports.default,
  "isDeveloper",
  { get: () => true },
);
```
This code will set the isDeveloper property to true.

# Test experiments
Finally, all we have to do is go into the settings and at the very bottom we'll see the Experiments tab. We click on that, and we'll see experiments. You always have a select menu where you can choose what type you want.




Credits to: 'https://hyro.pages.dev/blog/posts/how-to-try-discord-experiments/'
