# Hotel Amarante Orbital

Static marketing site for a fictional low-Earth-orbit hotel.

## Local preview

Open `index.html` in a browser, or serve the folder:

```bash
npx serve .
# or
python3 -m http.server 3000
```

## Deploy on Render

### Option A — Blueprint (recommended)

1. Push this folder to a GitHub/GitLab repo.
2. In [Render Dashboard](https://dashboard.render.com) → **New** → **Blueprint**.
3. Connect the repo. Render reads `render.yaml` and creates a Static Site.
4. Deploy. Your site will be at `https://amarante-orbital.onrender.com` (or your custom name).

### Option B — Manual Static Site

1. Push this folder to a Git repo.
2. **New** → **Static Site**.
3. Settings:
   - **Build Command:** leave empty (or `echo ready`)
   - **Publish Directory:** `.` (root of the repo)
4. Create Static Site → wait for deploy.

### Custom domain

In the Render service → **Settings** → **Custom Domains** → add your domain and follow DNS instructions.

## Structure

```
.
├── index.html      # Full page (HTML + CSS + JS)
├── img/            # All photos
├── render.yaml     # Render blueprint
└── README.md
```

All image paths are relative (`img/...`), so the site works as long as `index.html` and `img/` stay together.
