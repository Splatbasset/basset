# splatbasset.dev

A static coding-education website built with **pure HTML and CSS** (no frameworks, no build step). Ready to host on **GitLab Pages**.

## Pages
- `index.html` — Home / landing page
- `courses.html` — Course catalog (Java, HTML, CSS, C#)
- `about.html` — About splatbasset
- `styles.css` — All styling and CSS animations
- `favicon.svg` — Site icon

## Colors
- Navy `#0a1628`
- White `#ffffff`
- Green `#00ff88`

Fonts (DM Sans + JetBrains Mono) are loaded from Google Fonts via `<link>` tags, so no local font files are needed.

## Preview locally
Just open `index.html` in a browser, or run a tiny static server:
```bash
python3 -m http.server 8080
```
Then visit http://localhost:8080

## Deploy to GitLab Pages
1. Create a new project on GitLab and push these files to the default branch.
2. The included `.gitlab-ci.yml` copies the site into a `public/` folder, which GitLab Pages serves automatically.
3. After the pipeline runs, your site is live at the URL shown under **Deploy → Pages** in your GitLab project settings.

### Using a custom domain (splatbasset.dev)
In your GitLab project go to **Deploy → Pages → New Domain**, add `splatbasset.dev`, and follow the DNS instructions GitLab provides at your domain registrar.
