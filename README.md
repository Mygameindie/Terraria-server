# Terraria Server Generator

A 100% client-side web tool that generates a Windows launcher (`StartServer.bat`)
and a `serverconfig.txt` for running a Terraria Dedicated Server.

Configure your world name/path, max players, port, password, character security,
and an **auto-restart-on-crash** option, then download the files and drop them
into your Terraria Server folder.

## Hosting it on a home PC (and joining from iPad)

See **[HOW-TO-HOST.md](HOW-TO-HOST.md)** for the full step-by-step: installing the
dedicated server, running the auto-restart launcher, port forwarding, and joining
from an iPad/mobile by IP.

The **Auto-restart** option is the fix for "my server keeps crashing" — the
launcher relaunches the server automatically a few seconds after any crash.

## Run it

It's a single static `index.html` — just open it in any browser, no build step.

## Hosting (GitHub Pages) — one-time setup

This repo serves as a static site. Publishing takes one click from the repo owner
(only the owner can turn Pages on the first time):

1. Go to **Settings → Pages** in the GitHub repository.
2. Under **Build and deployment → Source**, choose **Deploy from a branch**.
3. Branch: **`claude/terraria-server-generator-Jb5vh`** (or `main`), Folder: **`/ (root)`** → **Save**.
4. Wait ~1 minute. Your page goes live at:
   `https://mygameindie.github.io/Terraria-server/`

## Privacy

The tool runs entirely in your browser. No data, passwords, or IP addresses
are sent anywhere.

> Not affiliated with Re-Logic. Terraria is a trademark of Re-Logic.
