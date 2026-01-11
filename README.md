# MonoDesk Landing Pages

Landing pages for MonoDesk with early access booking via Google Calendar.

## Live Site

🔗 **https://landing.monodesk.com**

## Project Structure

```
monodesk-landing/
├── index.html                  # Navigation hub for all landing pages
├── counter-positioning.html    # "This might look like a PM tool" messaging
├── removing-the-admin.html     # "Make space for creativity" messaging
├── space-for-creativity.html   # Creative-focused messaging
├── tell-it-like-it-is.html     # Direct/honest messaging
├── bundle.html                 # Suite/bundle value prop
├── css/
│   ├── index.css
│   ├── counter-positioning.css
│   ├── removing-the-admin.css
│   ├── space-for-creativity.css
│   ├── tell-it-like-it-is.css
│   └── bundle.css
├── assets/                     # Shared images, icons, logos
├── backup/                     # Legacy/archived pages
│   ├── design-tokens.html
│   ├── example.html
│   ├── example-landing-01.html
│   └── example-landing-02.html
└── README.md
```

## CSS Architecture

**Each page has its own CSS file** - stylesheets are not shared between pages. This keeps each landing page variant independent and easily customizable.

| Page | CSS File |
|------|----------|
| `index.html` | `css/index.css` |
| `counter-positioning.html` | `css/counter-positioning.css` |
| `removing-the-admin.html` | `css/removing-the-admin.css` |
| `space-for-creativity.html` | `css/space-for-creativity.css` |
| `tell-it-like-it-is.html` | `css/tell-it-like-it-is.css` |
| `bundle.html` | `css/bundle.css` |

Assets in `/assets` can be shared across all pages.

## Analytics

- **Hotjar** - Heatmaps and session recordings (all pages)
- **Plausible** - Privacy-friendly analytics with custom event tracking for CTA clicks

## Getting Started

### Local Development

1. Clone the repository:
   ```bash
   git clone https://github.com/sparkworkspro/monodesk-landing.git
   cd monodesk-landing
   ```

2. Open in browser:
   - Simply open any `.html` file in your browser
   - Start with `index.html` for navigation

### Deployment

This project is deployed on **Vercel** and auto-deploys on push to `main`.

- **Production**: https://landing.monodesk.com
- **Preview**: Each PR gets a preview URL

## Tech Stack

- Pure HTML/CSS (no build step required)
- Google Calendar for appointment scheduling
- Hotjar for behavior analytics
- Plausible for privacy-friendly analytics
- Deployed on Vercel
