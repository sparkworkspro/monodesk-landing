# MonoDesk Landing Page

Simple landing pages for MonoDesk with early access booking.

## Live Site

🔗 **https://landing.monodesk.com/vibes.html**

## Project Structure

```
monodesk-landing/
├── example.html        # Example landing page
├── vibes.html          # Landing page (Vibes)
├── bundle.html         # Landing page (Bundle/Suite)
├── css/
│   ├── example.css     # Styles for example.html
│   ├── vibes.css       # Styles for vibes.html
│   └── bundle.css      # Styles for bundle.html
├── assets/
│   └── logo-lockup.svg # MonoDesk logo (shared)
└── README.md
```

## CSS Architecture

**Each page has its own CSS file** - stylesheets are not shared between pages. This keeps each landing page variant independent and easily customizable.

| Page | CSS File |
|------|----------|
| `example.html` | `css/example.css` |
| `vibes.html` | `css/vibes.css` |
| `bundle.html` | `css/bundle.css` |

Assets in `/assets` can be shared across all pages.

## Getting Started

### Local Development

1. Clone the repository:
   ```bash
   git clone https://github.com/sparkworkspro/monodesk-landing.git
   cd monodesk-landing
   ```

2. Open in browser:
   - Simply open any `.html` file in your browser

### Deployment

This project is deployed on **Vercel** and auto-deploys on push to `main`.

- **Production**: https://landing.monodesk.com
- **Preview**: Each PR gets a preview URL

## Tech Stack

- Pure HTML/CSS (no build step required)
- Deployed on Vercel
