# Udhav's List — PWA

Aesthetic, mobile-friendly todo app. Offline-ready. Saves to localStorage.

## Deploy options

### Netlify (drag & drop)
1. Go to https://app.netlify.com/drop
2. Drag the **entire folder** here (not the zip).
3. Open the site → Safari → Share → **Add to Home Screen**.

### GitHub Pages
1. Create a new repo (e.g., `udhavs-list`).
2. Upload *all* files in this folder to the repo root.
3. In repo Settings → Pages → set **Source = `main` /root**.
4. Open your Pages URL (e.g., `https://<you>.github.io/udhavs-list`) → Add to Home Screen in Safari.

### Vercel
1. Create a new project and **Import** the GitHub repo above.
2. Framework preset: **Other** (static). Build command: **None**. Output: **/**.
3. Deploy → open the URL → Add to Home Screen in Safari.

## Custom domain
- **Netlify**: Site settings → Domain management → Add custom domain. In your DNS, create a **CNAME** from `list.yourdomain.com` → your `*.netlify.app` domain.
- **Vercel**: Project → Settings → Domains → Add. In DNS, create a **CNAME** → `cname.vercel-dns.com`.

## Notes
- The service worker caches `index.html`, icons, and manifest for offline use.
- Data is stored locally in the browser (localStorage). Export/Import lives in the header.
