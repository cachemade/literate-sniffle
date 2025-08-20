# Website Starter (GitHub Pages Ready)

A minimal starter you can deploy on **GitHub Pages**. It includes:
- A landing page that shows your **logo**.
- Organized folders for **assets** (images, CSS, JS, fonts).
- Example pages (`/pages/about.html`, `/pages/contact.html`).
- A **redirect** example (`/redirects/old-page.html` → `/pages/about.html`).
- A `404.html` and `.nojekyll` for smooth GitHub Pages hosting.

---

## 🚀 Quick Start

1. **Download** this repo as a ZIP and unzip it.
2. Open the folder in **VS Code** → install the "Live Server" extension (optional but recommended).
3. Open `index.html` with Live Server to preview locally.

## 🖼 Replace the Logo

- Put your logo file in `assets/img/`.
- Update the `src` in `index.html` if needed:

  ```html
  <img src="assets/img/logo.svg" alt="My Logo" class="logo" />
  ```

You can keep `logo.svg` (editable text file) or replace it with `logo.png`/`logo.jpg`.
If you replace it, just make sure the `src` path matches your file name.

## 🧱 Folder Structure

```text
/ (root)
├── index.html
├── 404.html
├── .nojekyll
├── README.md
├── assets/
│   ├── css/styles.css
│   ├── js/main.js
│   └── img/
│       ├── logo.svg
│       ├── favicon.png
│       └── .gitkeep
├── pages/
│   ├── about.html
│   └── contact.html
└── redirects/
    └── old-page.html
```

- `assets/img/.gitkeep` ensures empty folders stay in Git.
- `assets/img/favicon.png` is a placeholder; replace it with a 32×32 or 64×64 icon if you like.

## ➕ Add New Pages

1. Copy `pages/about.html` and rename it (e.g., `pages/services.html`).
2. Change the `<title>` and page content.
3. Link to it from your nav or anywhere else:

   ```html
   <a href="pages/services.html">Services</a>
   ```

## 🔀 Redirects

If a page moved, you can redirect an old URL to a new one. Example included: `redirects/old-page.html` sends visitors to `/pages/about.html`.

How it works (inside `old-page.html`):

```html
<meta http-equiv="refresh" content="0;url=/pages/about.html" />
<script>window.location.replace("/pages/about.html");</script>
```

Create more redirects by copying that file and changing the target URL.

## 🎨 Customize Styles & Scripts

- Edit **`assets/css/styles.css`** to change colors, spacing, and layout.
- Add your JS to **`assets/js/main.js`** for interactivity.

## 🌐 Publish on GitHub Pages

1. Create a new GitHub repository (e.g., `my-website`).
2. Upload all files and folders to the repo.
3. Go to **Settings → Pages**.
4. Under **Source**, choose the `main` branch and **Save**.
5. Your site will be live at: `https://YOUR-USERNAME.github.io/REPO-NAME/`

If you want it at `https://YOUR-USERNAME.github.io/` (no repo name), create a repo named `YOUR-USERNAME.github.io` and upload this starter there.

## 🧪 Test Locally (Optional)

- With VS Code **Live Server**: right-click `index.html` → *Open with Live Server*.
- Or just double-click `index.html` to open it in your browser.

## ❓ FAQ

- **Where do I put images?** → `assets/img/`
- **How do I link to another page?** → Use relative paths like `pages/about.html`.
- **How do I change background color or fonts?** → Edit `assets/css/styles.css`.
- **Can I use a custom domain?** → Yes! Add a `CNAME` file with your domain in the repo settings and DNS.

---

Happy building! ✨
