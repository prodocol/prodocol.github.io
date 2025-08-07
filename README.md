# MySite Starter (GitHub Pages + Porkbun)

Everything you need to get a simple site online fast.

## Files
- `index.html` — a clean, single-file site template.
- `github-pages-dns.txt` — Porkbun DNS import prefilled for GitHub Pages (replace `USERNAME`).
- `README.md` — these instructions.

---

## 1) Put the site on GitHub Pages

1. Create a **public** GitHub repository named:
   ```
   USERNAME.github.io
   ```
   Replace `USERNAME` with your GitHub username.

2. From a terminal (Git Bash, macOS Terminal, or Linux shell) run:
   ```bash
   # unzip the starter and go into it
   unzip mysite-starter.zip
   cd mysite-starter

   # initialize the repo and push
   git init
   git add index.html
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/USERNAME/USERNAME.github.io.git
   git push -u origin main
   ```

3. In the GitHub repo, go to **Settings → Pages** and ensure:
   - **Build and deployment → Source** is set to **Deploy from a branch**
   - **Branch**: `main` / root

Your site will be live shortly at:
```
https://USERNAME.github.io
```

---

## 2) Point your Porkbun domain to GitHub Pages

1. Log into Porkbun → **Domain Management → yourdomain.com → DNS**.
2. Use **Bulk Edit / Import** and paste the contents of `github-pages-dns.txt`.
   - Replace `USERNAME` with your GitHub username *before* importing.
3. In GitHub **Settings → Pages**, set your **Custom domain** to `yourdomain.com`.
4. Check **Enforce HTTPS** once the certificate is issued.

DNS usually propagates within 10–60 minutes (can be faster).

---

## 3) Customize your site
- Edit the text in `index.html`.
- Replace the image `src` with your image URL, or upload an image to the repo and reference it like `./myimage.jpg`.
- Commit and push to update the live site.

---

**Timestamp:** 2025-08-07 21:43:07
