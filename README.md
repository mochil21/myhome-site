# MyHome GitHub Pages Deployment

This folder contains the static website for MyHome's Privacy Policy, Terms of Service, and landing page.

## Files

- `index.html` - Landing page with app features and download link
- `privacy.html` - Privacy Policy (required for Play Store)
- `terms.html` - Terms of Service

## Quick Deploy to GitHub Pages

### Option 1: Using GitHub (Recommended)

1. **Create a new GitHub repository:**
   ```
   Repository name: myhome-site
   Public (required for free GitHub Pages)
   ```

2. **Push these files:**
   ```bash
   cd c:\projects\myhome\gh-pages
   git init
   git add .
   git commit -m "Initial commit - Privacy Policy and Terms"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/myhome-site.git
   git push -u origin main
   ```

3. **Enable GitHub Pages:**
   - Go to repository Settings → Pages
   - Source: Deploy from a branch
   - Branch: main, folder: / (root)
   - Click Save

4. **Your site will be live at:**
   ```
   https://YOUR_USERNAME.github.io/myhome-site/privacy.html
   https://YOUR_USERNAME.github.io/myhome-site/terms.html
   ```

### Option 2: Using Existing nexusapps Repository

If you have a nexusapps.com repository with GitHub Pages already set up:

1. Copy these files to your existing repo's `myhome/` folder
2. Access at: `https://nexusapps.com/myhome/privacy.html`

## URLs for Play Store

After deployment, use these URLs in Google Play Console:

- **Privacy Policy URL:** `https://YOUR_USERNAME.github.io/myhome-site/privacy.html`
- **Terms of Service (optional):** `https://YOUR_USERNAME.github.io/myhome-site/terms.html`

## Custom Domain (Optional)

To use myhome.nexusapps.com:

1. Create a `CNAME` file with content: `myhome.nexusapps.com`
2. Add DNS record at your domain registrar:
   - Type: CNAME
   - Name: myhome
   - Value: YOUR_USERNAME.github.io

## Testing Locally

Open any HTML file directly in your browser to preview:
```
start index.html
```

Or use a local server:
```bash
python -m http.server 8080
# Then open http://localhost:8080
```
