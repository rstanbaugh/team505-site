# team505-site

Minimal, logo-driven company announcement site for deployment on Cloudflare Pages.

## Project Structure

- `index.html` - Main one-page site (Home + About section + contact info)
- `about.html` - Redirect to About section on `index.html`
- `styles.css` - Site styling and animations
- `assets/rsm-logo.png` - Company logo

## Local Preview

Because this is static HTML/CSS, you can preview with any static server.

### Option 1: Python

```bash
cd team505-site
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## Publish With Git + Cloudflare Pages

1. Create a new GitHub repository and push this folder.
2. In Cloudflare Dashboard, go to **Workers & Pages** -> **Create** -> **Pages** -> **Connect to Git**.
3. Select your GitHub repo and branch (usually `main`).
4. Build settings:
   - Framework preset: `None`
   - Build command: leave blank
   - Build output directory: `/` (root)
5. Save and deploy.

Cloudflare will auto-deploy on every new push to the selected branch.

## Optional Custom Domain

1. Open your Cloudflare Pages project.
2. Go to **Custom domains**.
3. Add your domain and follow DNS prompts.
