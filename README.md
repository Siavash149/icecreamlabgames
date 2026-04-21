# IcecreamLab Games — Website

Static Jekyll site with Decap CMS for visual editing.

## Deploy to GitHub Pages (step by step)

### 1. Create GitHub repo
- Go to github.com → New repository
- Name it: `icecreamlabgames`
- Set to **Public**
- Do NOT initialize with README

### 2. Upload these files
```bash
git init
git add .
git commit -m "Initial site"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/icecreamlabgames.git
git push -u origin main
```

### 3. Enable GitHub Pages
- Go to repo → Settings → Pages
- Source: **Deploy from a branch**
- Branch: **main** / **(root)**
- Save

Your site will be live at `https://YOUR_USERNAME.github.io/icecreamlabgames` in ~2 minutes.

### 4. Set up custom domain
- In GitHub Pages settings → Custom domain → type `icecreamlabgames.com`
- On Parspack DNS panel add:
  - Type: `A` | Name: `@` | Value: `185.199.108.153`
  - Type: `A` | Name: `@` | Value: `185.199.109.153`
  - Type: `A` | Name: `@` | Value: `185.199.110.153`
  - Type: `A` | Name: `@` | Value: `185.199.111.153`
  - Type: `CNAME` | Name: `www` | Value: `YOUR_USERNAME.github.io`

### 5. Set up the CMS (Decap)

**Edit `admin/config.yml` first:**
Replace `YOUR_GITHUB_USERNAME` with your actual GitHub username.

**Set up GitHub OAuth App:**
1. Go to github.com → Settings → Developer settings → OAuth Apps → New OAuth App
2. Fill in:
   - Application name: `IcecreamLab CMS`
   - Homepage URL: `https://icecreamlabgames.com`
   - Authorization callback URL: `https://icecreamlabgames.com/admin/`
3. Click Register
4. Copy the **Client ID** — you don't need to do anything else with it, PKCE handles the auth client-side

**Add Client ID to CMS config:**
In `admin/config.yml`, add under `backend`:
```yaml
backend:
  name: github
  repo: YOUR_USERNAME/icecreamlabgames
  branch: main
  auth_type: pkce
  app_id: YOUR_GITHUB_OAUTH_CLIENT_ID
```

### 6. Access the CMS
Go to `https://icecreamlabgames.com/admin/`
Click "Login with GitHub" — done.

## What you can edit in the CMS
- **Games** — add/remove/edit any game (name, description, rating, Play Store link, icon)
- **Site Settings** — studio name, tagline, emails, Play Store URL
- **Pages** — Privacy Policy and Support FAQ text
- **Images** — upload via the media library button in the CMS

## Adding a new page
For now, new pages need a file added manually. Ask Claude to generate it.
Full visual page creation can be added later with more CMS config.
