# RasToken Website

A modern, animated website for RasToken (RasT) - the official token for the SuperOperatingSystem ecosystem.

## Features

**Modern Design**
- Vibrant blue color scheme matching the RasToken logo
- Smooth animations and transitions
- Fully responsive design
- Mobile-friendly interface

**Comprehensive Content**
- What is RasT? - Introduction to the token
- Why Different - Comparison with traditional tokens
- Core Features - 6 key features explained
- Ecosystem Overview - How everything works together
- Technology Stack - Modern infrastructure details

**Interactive Elements**
- Smooth scroll navigation
- Floating particle animations
- Scroll-triggered reveals
- Hover effects on cards
- Button ripple effects
- Parallax scrolling

## Project Structure

```
RasToken/
├── index.html       # Main website page
├── style.css        # Styling with animations
├── script.js        # Interactive functionality
├── logo.jpg         # RasToken logo
└── README.md        # This file
```

## Quick Start

### Local Development

1. Clone or download the repository
2. Open `index.html` in your web browser
3. The site will work offline with all animations and interactions

### GitHub Pages Setup

#### Option 1: Deploy from main branch

1. Push your files to GitHub repository
2. Go to **Settings** → **Pages**
3. Select **Main branch** as source
4. Click **Save**
5. Your site will be live at `https://yourusername.github.io/RasToken`

#### Option 2: Deploy from docs folder

1. Create a `docs` folder and move all files there
2. Push to GitHub
3. Go to **Settings** → **Pages**
4. Select **main branch /docs folder** as source
5. Click **Save**

#### Option 3: Use GitHub Actions for automatic deployment

Create `.github/workflows/deploy.yml`:

```yaml
name: Deploy to GitHub Pages

on:
  push:
    branches:
      - main

jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - name: Deploy
        uses: peaceiris/actions-gh-pages@v3
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          publish_dir: ./
```

## Customization

### Colors
Edit the CSS variables in `style.css`:
```css
:root {
    --primary-blue: #0066FF;
    --dark-navy: #001a4d;
    --darker-navy: #000d26;
    --light-blue: #1a7fff;
    --accent-white: #ffffff;
}
```

### Content
Edit the HTML sections in `index.html`:
- Update text content in each `<section>`
- Modify links in the footer
- Customize the navigation menu

### Animations
Adjust animation speeds and effects in `style.css`:
```css
--transition: all 0.3s cubic-bezier(...);
animation: slideDown 0.6s ease-out;
```

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Performance

- Fully responsive design
- Optimized animations using CSS
- No external dependencies
- Fast loading times
- SEO-friendly structure

## Social Links

- **GitHub**: [github.com/rastoken](https://github.com/rastoken)
- **Twitter/X**: [@TokenRas](https://x.com/TokenRas)

## License

This website is part of the RasToken project. All rights reserved.

## Support

For issues or suggestions, please contact:
- Email: contact@rastoken.io
- Website: rastoken.io

---

**Built with 💙 for the RasToken Community**

Version: 1.0.0
Last Updated: 2026
