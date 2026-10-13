# GGNodes Modern Panel UI

A single-file, responsive Minecraft hosting control-panel frontend prototype.

## Included
- Modern dark UI with transitions, animated aurora, hover effects, and responsive layout.
- Appearance page with photo and video background uploads, dim/blur controls, and ambient animation toggle.
- Browser-local background persistence using IndexedDB where supported.
- Blueprint gallery: Paper SMP, Vanilla Survival, Lifesteal SMP, BoxPvP Arena, Fabric Mods, Forge Modpack, and Velocity Proxy.
- Dashboard, console preview, demo file listing, backup entries, and display settings.

## Publish with GitHub Pages
1. Create a GitHub repository, e.g. `ggnodes-panel`.
2. Upload `index.html` to the repository root and commit it.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, branch `main`, folder `/(root)`, then save.
5. Open the GitHub Pages URL shown there.

## Important limitations
This is a frontend-only demo. Start/stop/restart actions, console commands, files, backups, and blueprint deployment are simulated. GitHub Pages cannot run Minecraft server processes or safely store server secrets. A production system needs a secured backend and server-management service (for example, an appropriately configured Pterodactyl/Wings integration), authentication/authorization, resource validation, and protected API credentials. Never put admin API keys in client-side code.

Background photo/video files are stored in the visitor's own browser where IndexedDB is supported; they are not uploaded to GitHub or shared with other panel users. A remote background URL must point directly to a media file and allow embedding.
