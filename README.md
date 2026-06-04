# Terraria Server Generator

A 100% client-side web tool that generates a Windows launcher (`StartServer.bat`)
and a `serverconfig.txt` for running a Terraria Dedicated Server.

Configure your world name/path, max players, port, password, and character
security, then download the files and drop them into your Terraria Server folder.

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
