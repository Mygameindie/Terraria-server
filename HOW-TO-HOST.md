# How to host your own Terraria server on a home PC (and join from iPad)

You play Terraria on **iPad**, but a server has to run on a **computer that stays on**.
Your iPad just *joins* it by IP — exactly like you did on the free host (mc4.in).
The difference: this one is **yours**, and the launcher **auto-restarts if it crashes**.

> ⚠️ **Version must match.** Your PC Terraria Dedicated Server and your iPad's
> Terraria app must be the **same version** (e.g. both 1.4.4.x). If versions differ,
> the iPad can't connect — update both to the latest.

---

## Part 1 — Set up the server on the PC

1. On the PC, open **Steam → Library**. Use the top filter and switch it to **Tools**.
2. Find **Terraria Dedicated Server** → **Install**.
3. Open this generator (the web page), fill in:
   - **World** name, **Max Players**, **Port** = `7777`, a **Password**, keep
     **Auto-restart** checked.
4. Click **⬇️ Download .bat**.
5. Find the server folder: right-click **Terraria Dedicated Server** in Steam →
   **Manage → Browse local files**. It's the folder containing `TerrariaServer.exe`.
6. Move `StartServer.bat` into that folder.
7. **Double-click `StartServer.bat`.** When you see "Starting server..." it's live.
   If it ever crashes, it now relaunches itself in 5 seconds. ✅

Leave that window open the whole time people are playing. Closing it = server off.

---

## Part 2 — Let your iPad (and friends) join

### A) Same Wi-Fi as the PC (easiest)
1. Find the PC's local IP: open **Command Prompt**, type `ipconfig`, read **IPv4 Address**
   (looks like `192.168.1.20`).
2. On the iPad: **Terraria → Multiplayer → Join via IP** → enter that IP and port `7777`
   → type the password. Done. 🎮

### B) Friends in other houses (over the internet)
The server's home router must let traffic in:
1. **Port forward** TCP (and UDP) port `7777` on the PC's router to the PC's local IP
   (the `192.168.x.x` from above). This is done in the router's admin page
   (usually `192.168.1.1` in a browser → "Port Forwarding").
2. Find your **public IP**: google "what is my IP" on the PC.
3. Friends use **Join via IP** with that **public IP** + port `7777` + password.

> Prefer not to touch the router? On the **PC** you can install a free virtual-LAN
> app (Radmin VPN / Hamachi) and have friends connect through it — but note those
> apps don't run on iOS, so this only helps PC players, not iPad friends. For iPad
> friends over the internet, port forwarding is the reliable route.

---

## Why this fixes your crashing problem
- Free hosts (like mc4.in) throttle, sleep, and crash without recovering.
- Your `StartServer.bat` runs an **auto-restart loop**: if `TerrariaServer.exe`
  exits for any reason, it waits 5 seconds and starts again — so a crash becomes
  a brief blip instead of "server is down."

## Keeping it always-on
A home PC works, but it must stay powered on. If you'd rather not leave a PC
running 24/7, the same files + idea work on a rented host or a free cloud VPS —
ask and we can set that up next.
