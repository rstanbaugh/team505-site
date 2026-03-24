# team505-site

Minimal, logo-driven company site deployed on Cloudflare Pages.

## Live Site

- https://team505.ai
- https://www.team505.ai

## Project Structure

- `index.html` - Main one-page site (Home + About section + contact info)
- `about.html` - Redirect to About section on `index.html`
- `styles.css` - Site styling and animations
- `assets/rsm-logo-1.png` - Primary logo currently used on the site

## Local Preview

Because this is static HTML/CSS, you can preview with any static server.

### Option 1: Python

```bash
cd team505-site
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## Deployment Workflow

Deployment is connected to GitHub through Cloudflare Pages and deploys automatically on push.

1. Edit files locally.
2. Run `git add .`.
3. Run `git commit -m "..."`.
4. Run `git push`.
5. Cloudflare Pages detects the push.
6. Cloudflare Pages rebuilds and deploys automatically.

No manual deploy step is required after push.

## Optional Custom Domain

1. Open your Cloudflare Pages project.
2. Go to **Custom domains**.
3. Add your domain and follow DNS prompts.
