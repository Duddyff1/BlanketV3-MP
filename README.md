# Blanket Multiplayer — GitHub Pages starter

This is a recreated starter based on the Blanket features described in chat. It is **not your original source code**; your original project files were not attached here, so I rebuilt the known features into this version.

## Included
- Packs, including Fall and other seasonal packs; no market
- 5,200 generated collectible entries, pack assignment, rarity labels and Secret collection
- My Blankies inventory with search and sorting
- Three distinct quiz modes
- Coins and collection saved in the browser
- Multiplayer room codes, player list, scores and group quiz hooks
- Demo admin panel for local testing

## Publish on GitHub Pages
1. Unzip this folder.
2. Create/open your GitHub repository.
3. Upload `index.html`, `app.js`, `firebase-config.js`, `firebase-database-rules.json`, and this README to the repository root.
4. Open repository **Settings → Pages**, select **Deploy from a branch**, choose `main` and `/ (root)`, then Save.

## Enable real multiplayer across different devices
The game uses Firebase Realtime Database for online rooms. It will show local/demo mode until configured.

1. In Firebase Console, create a project and add a Web App.
2. Create a **Realtime Database**.
3. Copy the Firebase web config into `firebase-config.js`, replacing every `YOUR_...` value and `PASTE_API_KEY_HERE`.
4. In Realtime Database Rules, start with the rules in `firebase-database-rules.json` **only for quick private testing**.

### Important security note
The included open database rules are insecure and are for short private tests only. Anyone who knows the site could read or change room data. Before making the game public, use Firebase Authentication and restrictive rules. The admin panel is local-only demo controls; it does not securely grant real admin privileges. Never put a Firebase service-account key or other private server secret in this website.

## Limitations
- Because your original files were not supplied, this build reconstructs the described features rather than preserving your exact old code, artwork, pack data, admin settings, or progress.
- The 5,200 catalog entries are generated starter content, not 5,200 individually hand-designed official items.
- The browser save is local to each browser/device. It does not migrate existing saves or collections.
