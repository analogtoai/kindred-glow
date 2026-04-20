# Kindred Glow — Deployment Package
_Built with love. Ready to drop into Netlify._

## What's in this folder

| File/Folder | Purpose |
|---|---|
| `index.html` | Home page / landing |
| `about.html` | About the Sanctuary |
| `support.html` | Support & The Keeper's Guide |
| `legal.html` | Privacy Policy & Terms |
| `manifest.json` | PWA install config (enables "Add to Home Screen") |
| `sw.js` | Service Worker (offline support + installability) |
| `icons/` | App icons (192px and 512px) |
| `netlify.toml` | Netlify configuration (caching, headers) |

## How to deploy

### Option A: Netlify Drag & Drop (easiest)
1. Go to [app.netlify.com](https://app.netlify.com)
2. Click **"Add new site" → "Deploy manually"**
3. Drag this entire `kindred_glow` folder into the upload box
4. Done — you'll get a live `.netlify.app` URL in ~30 seconds

### Option B: GitHub → Netlify (recommended for updates)
1. Create a new GitHub repo (e.g. `kindred-glow-site`)
2. Push this folder's contents as the root of the repo
3. In Netlify: **"Add new site" → "Import from Git"** → connect the repo
4. Every time you push to GitHub, Netlify auto-deploys

## Connecting your custom domain
1. In Netlify: **Site settings → Domain management → Add custom domain**
2. Enter your domain (e.g. `kindredglow.ai`)
3. Netlify will give you nameservers OR a CNAME record
4. In Cloudflare: add the CNAME record pointing to your Netlify URL
5. SSL is automatic — Netlify provisions it via Let's Encrypt

## PWA "Add to Home Screen"
Once deployed to HTTPS (your custom domain), users can install it:
- **iOS Safari**: Share button → "Add to Home Screen"
- **Android Chrome**: Three-dot menu → "Add to Home Screen" (or the automatic install banner)
- **Desktop Chrome/Edge**: Install icon in the address bar

## Replacing the placeholder icon
The current icon (`icons/icon-192.png` and `icon-512.png`) is a placeholder.
To use your real brand icon:
1. Create a square PNG at 512×512px with your logo
2. Replace both files in the `icons/` folder
3. Re-deploy

---
_Kindred Glow — Connection, at your own pace._
