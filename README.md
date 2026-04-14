# NUE Urban Concepts Website

Redesigned website for **NUE Urban Concepts** — Land Use · Mobility · Parking · Fees.

## File Structure

```
nue-urban-concepts/
├── index.html                  # Home / landing page
├── about.html                  # About Us
├── our-work.html               # Portfolio of projects
├── innovation.html             # Innovation initiatives
├── mobility-cohort.html        # Mobility Cohort program
├── mobility-fee-database.html  # Searchable mobility fee database
├── contact.html                # Contact form + office locations
├── css/
│   └── styles.css              # All styles (dark theme, brand colors)
├── js/
│   └── scripts.js              # Nav, scroll animations, form handler
└── images/
    ├── logo-white.png          # White logo (used on dark backgrounds)
    └── logo-dark.png           # Dark logo (for light contexts)
```

## Hosting on GitHub Pages

1. Push all files to a GitHub repository
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)` folder
4. Your site will be live at `https://yourusername.github.io/repo-name`

> For a custom domain (nueurbanconcepts.com), add a `CNAME` file with your domain and configure DNS with your registrar.

## Customization Notes

### Adding Project Images (Our Work page)
Replace `.project-placeholder` divs in `our-work.html` with:
```html
<img src="images/project-name.jpg" alt="Project description" class="…">
```
Recommended image size: **800×600px**, JPG or WebP.

### Team Photos (About Us page)
Replace `.team-photo-placeholder` divs with:
```html
<img src="images/team-name.jpg" alt="Name" class="team-photo">
```

### Contact Form
The form currently simulates a submission. To connect it to a real backend:
- **Netlify Forms**: Add `netlify` attribute to the `<form>` tag
- **Formspree**: Set `action="https://formspree.io/f/YOUR_ID"` and `method="POST"`
- **EmailJS**: Replace the setTimeout in `scripts.js` with EmailJS SDK calls

### Brand Colors
All colors are CSS variables in `css/styles.css`:
```css
--green:        #145703;   /* Primary brand green */
--green-light:  #1d7a04;   /* Hover states */
--green-glow:   #2a9e06;   /* Accents & labels */
--dark:         #0d0d0d;   /* Page background */
```

### Google Fonts
The site uses **Barlow Condensed** (headings) and **Barlow** (body) loaded from Google Fonts. An internet connection is required to load these fonts. For offline use, download and self-host them.

## Browser Support
Chrome, Firefox, Safari, Edge (last 2 versions). Fully responsive for mobile, tablet, and desktop.
