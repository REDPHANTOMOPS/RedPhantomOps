# GitHub Pages Setup for redphantomops.com

This repository is configured to host a website using GitHub Pages with a custom domain.

## What's Included

- **index.html**: The main landing page with company information
- **style.css**: Professional styling with responsive design
- **CNAME**: Custom domain configuration file

## GitHub Pages Configuration

To enable GitHub Pages for this repository:

1. Go to your repository settings on GitHub
2. Navigate to "Pages" in the left sidebar
3. Under "Source", select the branch you want to deploy (e.g., `main` or `copilot/build-website-for-redphantomops`)
4. Select the root folder (`/`) as the source
5. Click "Save"

## Custom Domain Setup

The CNAME file is already configured with `redphantomops.com`. To complete the setup:

### DNS Configuration

Add the following DNS records in your domain registrar's DNS settings:

#### For Apex Domain (redphantomops.com):
Add these A records:
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

#### For www Subdomain:
Add a CNAME record:
```
CNAME: www.redphantomops.com -> REDPHANTOMOPS.github.io
```

### GitHub Pages Custom Domain

1. In GitHub repository settings → Pages
2. Under "Custom domain", enter: `redphantomops.com`
3. Click "Save"
4. Wait for DNS check to complete (may take a few minutes)
5. Once verified, enable "Enforce HTTPS" for secure connections

## Website Features

- **Responsive Design**: Works on desktop, tablet, and mobile devices
- **Modern UI**: Clean, professional design with smooth animations
- **Section Navigation**: Home, About, Services, and Contact sections
- **SEO Ready**: Includes meta tags for search engines

## Customization

To customize the website:

1. Edit `index.html` to change content, sections, or structure
2. Modify `style.css` to adjust colors, fonts, or layout
3. Update the contact information and company details

## Troubleshooting

- **DNS Propagation**: DNS changes can take up to 48 hours to propagate globally
- **HTTPS**: Allow time for GitHub to provision an SSL certificate after domain verification
- **404 Error**: Ensure the branch is correctly configured in GitHub Pages settings

## Support

For issues or questions, please open an issue in this repository.
