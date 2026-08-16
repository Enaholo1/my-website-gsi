# Global Secure Intelligence website

A responsive, dependency-free marketing site for **Global Secure Intelligence**.

## Files

- `index.html` — homepage
- `services.html`, `about.html`, `contact.html` — main pages
- `styles.css` and `script.js` — styling and interaction
- `netlify.toml` — Netlify configuration
- `CNAME` — custom domain for GitHub Pages

## Run locally

No build step is required. Open `index.html` in a browser, or from this folder run:

```sh
python3 -m http.server 8080
```

Then visit <http://localhost:8080>.

## Deploy from GitHub

1. Create an empty GitHub repository, such as `gsi-website`.
2. Commit and push this folder’s contents to the repository:

```sh
git init
git add .
git commit -m "Launch Global Secure Intelligence website"
git branch -M main
git remote add origin https://github.com/YOUR-ACCOUNT/gsi-website.git
git push -u origin main
```

3. In Netlify, choose **Add new site → Import an existing project → GitHub**, then select the repository.
4. Keep the build command empty and set the publish directory to `.`. The included `netlify.toml` already supplies this configuration.
5. Under **Domain management**, add `globalsecureintelligence.com` and follow Netlify’s DNS instructions.

The contact form is marked for [Netlify Forms](https://docs.netlify.com/manage/forms/setup/). Once the site is deployed on Netlify, submissions will appear in the Netlify Forms dashboard. If a different platform is used, connect its preferred form provider or backend to `contact.html`.

## Before launch

- Confirm the phone number and email address in the site footer and contact page.
- Configure the DNS records with the chosen deployment platform.
- Add an analytics or cookie policy only if one is actually needed.
