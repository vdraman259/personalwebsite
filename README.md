# Raman Namboodiripad — Portfolio

A dark space-themed personal portfolio built with pure HTML, CSS, and vanilla JavaScript. No frameworks. No build step. Just drop and deploy.

## ✦ Live Site

> `https://<your-github-username>.github.io/<repo-name>/`

---

## 📁 File Structure

```
portfolio/
├── index.html       ← Main portfolio page (all-in-one)
├── .nojekyll        ← Disables GitHub's Jekyll processing
└── README.md        ← This file
```

---

## 🚀 Deploy to GitHub Pages

### 1. Create a new GitHub repository
- Go to [github.com/new](https://github.com/new)
- Name it `portfolio` (or anything you like)
- Set visibility to **Public**
- Click **Create repository**

### 2. Upload your files
**Option A — via GitHub UI (easiest):**
1. On your new repo page, click **Add file → Upload files**
2. Drag and drop `index.html`, `.nojekyll`, and `README.md`
3. Click **Commit changes**

**Option B — via Git CLI:**
```bash
git init
git add .
git commit -m "Initial portfolio upload"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```

### 3. Enable GitHub Pages
1. In your repo, go to **Settings → Pages**
2. Under **Source**, select **Deploy from a branch**
3. Set branch to `main` and folder to `/ (root)`
4. Click **Save**

### 4. Visit your live site
After ~60 seconds, your site will be live at:
```
https://<your-github-username>.github.io/<repo-name>/
```

---

## 🌐 Custom Domain (Optional)

To use your own domain (e.g. `raman.dev`):

1. In **Settings → Pages**, enter your domain under **Custom domain**
2. Add a `CNAME` file to your repo root containing just your domain:
   ```
   raman.dev
   ```
3. At your domain registrar, add a CNAME DNS record:
   - **Host:** `www`
   - **Points to:** `<your-github-username>.github.io`
4. For the apex domain (`raman.dev`), add 4 A records pointing to GitHub's IPs:
   ```
   185.199.108.153
   185.199.109.153
   185.199.110.153
   185.199.111.153
   ```

---

## ✏️ Customisation Notes

| What to change | Where in index.html |
|---|---|
| Your name / logo | `.logo` text → `Raman.N` |
| Social links | `href` on `.s-btn` and `.cta-s-btn` buttons |
| Hero headline | `<h1 class="hero-heading">` |
| About bio text | `<p class="about-desc">` |
| Project card labels | `.rarity-val` inside each `.nft-card` |
| Background videos | `<source src="...">` in each section |
| Accent colour (neon green) | `#6FFF00` → find & replace in `<style>` |

---

## 🛠 Tech Stack

- **HTML5 / CSS3** — no frameworks
- **Google Fonts** — Anton + Condiment
- **Videos** — served from AWS CloudFront
- **Hosting** — GitHub Pages (free)
