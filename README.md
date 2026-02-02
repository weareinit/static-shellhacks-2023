# ShellHacks 2023 - Static Site

This branch contains the static export of the ShellHacks 2023 landing page for deployment to GitHub Pages.

## Deployment Information

- **Custom Domain**: 2023.shellhacks.net
- **Branch**: github-pages
- **Deployment Method**: GitHub Actions (automatic on push)

## Local Testing

To test the static site locally:

```bash
npx serve .
```

Then visit http://localhost:3000 in your browser.

## File Structure

- `index.html` - Main landing page
- `_next/` - Next.js static assets (CSS, JS chunks)
- `assets/` - Images and decorations
- `fonts/` - Custom fonts
- `images/` - Favicon and social images
- `.nojekyll` - Prevents GitHub Pages from using Jekyll
- `CNAME` - Custom domain configuration
- `.github/workflows/deploy.yml` - GitHub Actions deployment workflow

## Updating the Site

To update the static site:

1. Switch back to `main` branch
2. Make your changes
3. Run `npm run export` to rebuild static files
4. Switch to `github-pages` branch
5. Copy new files from `out/` directory
6. Commit and push

The GitHub Actions workflow will automatically deploy the changes.

## Site Features

- ✅ Static HTML export from Next.js
- ✅ All images and assets optimized
- ✅ Custom fonts included
- ✅ Event information (September 15-17, 2023)
- ✅ "Event ended" message (registration removed)
- ✅ About Us, FAQ, Sponsors sections
- ✅ Social media links
- ✅ Responsive design

## Total Size

~9.7 MB (well within GitHub Pages limits)
