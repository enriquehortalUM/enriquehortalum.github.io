# Enrique Hortal Quesada — Academic Personal Site

A minimalist, modern academic personal website built with plain HTML and CSS — no frameworks, no build tools. Ready to deploy on GitHub Pages in one push.

---

## 📁 File structure

```
enrique-hortal-site/
├── index.html            ← Main page (About, Experience, Education, Projects, Publications, Contact)
├── more.html             ← Extended content (journal collaborations, prizes, conferences, press)
├── assets/
│   └── css/
│       └── style.css     ← All styles
└── README.md
```

---

## 🚀 Deploy to GitHub Pages

### Option A — New repository

1. Create a new repository on GitHub (e.g. `enrique-hortal` or `your-username.github.io`)
2. Upload all files (or push via Git):

```bash
git init
git add .
git commit -m "Initial site"
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
git push -u origin main
```

3. Go to **Settings → Pages → Source** and select `main` branch, root `/`
4. Your site will be live at `https://YOUR_USERNAME.github.io/YOUR_REPO/`

### Option B — User/organisation page (recommended)

Name the repository `YOUR_USERNAME.github.io`. The site will be served at `https://YOUR_USERNAME.github.io` automatically.

---

## 📸 Profile photo

The photo currently loads from the original WordPress URL. For better reliability, download it locally:

1. Download your photo and save it as `assets/img/enrique-hortal.jpg`
2. In `index.html`, replace:
   ```
   src="https://dke.maastrichtuniversity.nl/.../DSCF1759-copia.jpg"
   ```
   with:
   ```
   src="assets/img/enrique-hortal.jpg"
   ```

---

## ✏️ Updating content

All content is in plain HTML — just open the files in any text editor and update:

- **Bio / About**: `index.html` → `#about` section
- **Publications**: `index.html` → `#publications` section
- **More content**: `more.html`
- **Colors / fonts**: `assets/css/style.css` → `:root` variables

---

## 🎨 Design tokens (quick customisation)

In `assets/css/style.css`, find `:root` and adjust:

| Variable | Default | Purpose |
|---|---|---|
| `--accent` | `#1D4A8A` | Navy blue accent color |
| `--font-display` | Playfair Display | Serif headings |
| `--font-body` | Inter | Body text |
| `--bg-alt` | `#F7F8FA` | Alternating section background |

Fonts are loaded from Google Fonts — no local installation needed.

---

## 🌐 Custom domain (optional)

To use a custom domain (e.g. `enriquehortal.com`):

1. Add a `CNAME` file in the root with your domain name:
   ```
   enriquehortal.com
   ```
2. Configure your domain DNS to point to GitHub Pages (see [GitHub Pages docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site))
