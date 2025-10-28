
# VibeForward Media — Git + Netlify Starter

This repo contains a single static `index.html` using Tailwind via CDN. No build step needed.

## Deploy to Netlify (from Git)
1. Create a new GitHub repo (e.g., `vibeforward-site`).
2. Upload these files (`index.html`, `netlify.toml`).
3. In Netlify: **New site from Git → GitHub → select repo**.
4. Build settings:
   - **Build command**: _leave empty_
   - **Publish directory**: `.`
5. Click **Deploy**. You're live!

## Quick Git commands
```bash
git init
git add .
git commit -m "Initial commit: VibeForward site"
git branch -M main
git remote add origin https://github.com/YOUR-USER/vibeforward-site.git
git push -u origin main
```

## Update workflow
- Edit `index.html` → `git commit` → `git push` → Netlify auto‑deploys.
- For previews, open pull requests; Netlify will generate a Deploy Preview link.

## Optional: Netlify Forms
To save form submissions to your Netlify dashboard, change your `<form>` tag to:
```html
<form name="contact" method="POST" data-netlify="true">
  <input type="hidden" name="form-name" value="contact" />
  ...
</form>
```
