# SnoreCatcher Website

SnoreCatcher developer website and privacy policy page.

## Project Structure

```
SnoreCatcherWebsite/
├── index.html          # Main page (product introduction)
├── privacy.html        # Privacy policy page
├── styles.css          # Stylesheet
├── README.md           # Project documentation
├── netlify.toml        # Netlify configuration (optional)
└── .gitignore          # Git ignore file
```

## Deploy to Netlify

### Method 1: Auto-deploy via Git connection

1. Push code to a Git repository (GitHub, GitLab, or Bitbucket)
2. Connect Git repository in Netlify dashboard
3. Build settings:
   - **Build command**: (leave empty, static site doesn't need build)
   - **Publish directory**: `/` or `.`
4. Click "Deploy site"

### Method 2: Manual deployment

1. In Netlify dashboard, select "Sites"
2. Click "Add new site" → "Deploy manually"
3. Drag and drop the entire folder to the deployment area

## Local Preview

You can use any static file server to preview the website:

### Using Python

```bash
# Python 3
python3 -m http.server 8000

# Then visit http://localhost:8000
```

### Using Node.js (http-server)

```bash
npx http-server -p 8000
```

### Using VS Code Live Server

Install the "Live Server" extension, right-click `index.html` and select "Open with Live Server"

## Customization

### Update App Store Link

In `index.html`, search and replace:
```html
<a href="https://apps.apple.com/app/snorecatcher" ...>
```

Replace with your actual App Store link.

### Modify Styles

Edit CSS variables in `styles.css` to customize color theme:
```css
:root {
    --primary-color: #2c3e50;
    --secondary-color: #3498db;
    --accent-color: #e74c3c;
    /* ... other variables */
}
```

### Add Developer Contact Information

In the footer section of `index.html` and `privacy.html`, you can add:
- Email address
- Social media links
- Other contact methods

## Notes

1. **App Store Link**: Make sure to update the App Store download link in `index.html` before publishing
2. **Privacy Policy**: You may need to adjust content in `privacy.html` based on actual app functionality
3. **SEO**: You can add more meta tags and Open Graph tags as needed
4. **Analytics**: If you want to add Google Analytics or other analytics tools, you can add the corresponding code in the `<head>` section

## License

Copyright © 2026 SnoreCatcher
