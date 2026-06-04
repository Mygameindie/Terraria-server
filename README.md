# Terraria Server Generator

A 100% client-side web tool that generates a Windows launcher (`StartServer.bat`)
and a `serverconfig.txt` for running a Terraria Dedicated Server.

Configure your world name/path, max players, port, password, and character
security, then download the files and drop them into your Terraria Server folder.

## Run it

It's a single static `index.html` — just open it in any browser, no build step.

## Hosting (GitHub Pages)

This repo is set up to be served as a static site. To publish it:

1. Go to **Settings → Pages** in the GitHub repository.
2. Under **Build and deployment → Source**, choose **Deploy from a branch**.
3. Select the branch containing `index.html` and the `/ (root)` folder, then **Save**.
4. Your page will be live at `https://<user>.github.io/terraria-server/`.

## Privacy

The tool runs entirely in your browser. No data, passwords, or IP addresses
are sent anywhere.

> Not affiliated with Re-Logic. Terraria is a trademark of Re-Logic.
