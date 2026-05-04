# OmniTool Studio Deployment Guide

## What this package includes

This ZIP contains the source code for the OmniTool Studio React/Vite website, including:

- Calculator, converter, and utility tools
- About, Contact, Privacy Policy, and Terms pages
- Ad placeholder slots
- `robots.txt`
- Placeholder `ads.txt`

The ZIP intentionally excludes `node_modules` because hosting platforms install dependencies automatically.

## Recommended public hosting path

1. Create a GitHub repository.
2. Upload this project code to the repository.
3. Create a Vercel or Netlify account.
4. Import the GitHub repository.
5. Use these build settings:
   - Install command: `npm install`
   - Build command: `npm run build`
   - Output directory: `dist/public`
6. Connect your custom domain in the hosting dashboard.

## Before applying to Google AdSense

1. Replace the Contact page placeholder with your public support email.
2. Add your real AdSense verification script inside `client/index.html` between `<head>` and `</head>`.
3. Replace `client/public/ads.txt` with your real AdSense publisher line, usually:

```txt
google.com, pub-YOUR_PUBLISHER_ID, DIRECT, f08c47fec0942fa0
```

4. Deploy the site to your custom domain.
5. Submit the domain in Google AdSense.

## Local development

```bash
npm install
npm run dev
```

Then open the local URL shown in the terminal.

## Production build

```bash
npm run build
```

The built static files will be in:

```txt
dist/public
```
