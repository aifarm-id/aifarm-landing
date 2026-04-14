# Aifarm Landing Page

Static landing page for Aifarm - Dairy Goat Farm Management Solution.

## Deployment to GitHub Pages

### Option 1: Deploy to Root Domain (aifarm.id)

1. Create a new GitHub repository named `your-username.github.io`
2. Upload all files from this folder to the repository root
3. Go to repository Settings → Pages
4. Select "main" branch as source
5. Your site will be available at `https://your-username.github.io`

### Option 2: Deploy to Subdirectory (aifarm.id/landing)

1. Create a new GitHub repository (any name)
2. Upload all files from this folder to the repository
3. Go to repository Settings → Pages
4. Select "main" branch and "/ (root)" as source
5. Your site will be available at `https://your-username.github.io/repository-name`

## Custom Domain Setup (aifarm.id)

### 1. DNS Configuration

Log in to your domain registrar (where you bought aifarm.id) and add:

**For root domain (aifarm.id):**
```
Type: A
Name: @
Value: 185.199.108.153
```
Add 3 more A records with these IPs:
- 185.199.109.153
- 185.199.110.153
- 185.199.111.153

**For www subdomain (optional):**
```
Type: CNAME
Name: www
Value: your-username.github.io
```

### 2. GitHub Pages Settings

1. Go to your repository Settings → Pages
2. Under "Custom domain", enter: `aifarm.id`
3. Click Save
4. Wait for DNS check to pass
5. Enable "Enforce HTTPS" (recommended)

## File Structure

```
landing/
├── index.html          # Main HTML file
├── CNAME              # Custom domain configuration
├── README.md          # This file
└── assets/            # Images and static assets
    ├── aifarm.png
    ├── about.png
    ├── growth.png
    ├── effectiveness.png
    ├── integrated.png
    ├── features.png
    ├── pricing-free.png
    ├── pricing-starter.png
    ├── pricing-business.png
    ├── pricing-ultimate.png
    └── partners/       # Partner logos
        ├── kominfo.png
        ├── kpri.png
        ├── kemenparekraf.png
        ├── amikom.png
        ├── 1000startup.png
        ├── indigo.png
        ├── bsc.png
        ├── rbtv.png
        └── radarjogja.png
```

## Local Preview

To preview the page locally before deploying:

1. Install Python (if not already installed)
2. Open terminal in this folder
3. Run: `python -m http.server 8000`
4. Open browser to: `http://localhost:8000`

Or use VS Code "Live Server" extension.

## Technologies Used

- Tailwind CSS 4 (via CDN)
- AOS Animation Library
- Swiper JS (carousel)
- Google Fonts (Open Sans, Poppins)

## Color Scheme

- Primary: Teal (#0d9488)
- Secondary: Sky Blue (#0ea5e9)
- Accent: Orange (#ff901c)

## Contact

For issues or updates, contact admin@aifarm.id
