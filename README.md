# Aida Sam – Portfolio

Static portfolio site for a graphic designer, built to be hosted on GitHub Pages and served from the custom domain `aidasam.com`.

## Files

- `index.html` – main landing page with introduction, about, projects grid and contact section.
- `styles.css` – shared styling for the home page and all project pages.
- `project-lume.html` – full case study page for the **LUME coffee & bakery** project, using `IMG_3745.jpg`.
- `project-02.html`, `project-03.html`, `project-04.html` – placeholder pages ready to be filled with future projects.
- `IMG_3745.jpg` – LUME campaign / packaging image.

## How to publish with GitHub Pages

1. Create a new public repository on GitHub, for example `aidasam-portfolio`.
2. On your computer, in this directory (`AI Projects/Aidasam website`), initialize git and push:

   ```bash
   cd "/Users/amirshahcheraghian/AI Projects/Aidasam website"
   git init
   git branch -M main
   git add .
   git commit -m "Initial portfolio"
   git remote add origin git@github.com:YOUR_USERNAME/aidasam-portfolio.git
   git push -u origin main
   ```

3. In GitHub, open **Settings → Pages** for the repository:
   - Under **Source**, choose **Deploy from a branch**.
   - Select **Branch: `main`**, folder **`/ (root)`**, and click **Save**.
   - After a minute or two, GitHub Pages will give you a URL like `https://YOUR_USERNAME.github.io/aidasam-portfolio/`.

## Connect `aidasam.com` to GitHub Pages

1. In the repository root on GitHub, click **Add file → Create new file** and create a file named `CNAME` (no extension) with this content:

   ```text
   aidasam.com
   ```

   Commit the file to `main`.

2. In your domain provider’s DNS settings for `aidasam.com`:
   - Create an **A record** for `@` pointing to these IPs (GitHub Pages):
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`
   - Create a **CNAME record** for `www` pointing to `YOUR_USERNAME.github.io`.

3. Back in GitHub, under **Settings → Pages**, set the **Custom domain** to `aidasam.com` and save. GitHub will provision HTTPS automatically (this can take some minutes).

Once DNS has propagated, visiting `https://aidasam.com` will load this portfolio.

