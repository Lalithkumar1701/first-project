# Navira Health Clinic — Frontend

A modern, responsive healthcare clinic website built with HTML, CSS, and vanilla JavaScript.

## What's Here

- **index.html** — Complete website (single file for simplicity)
- **assets/** — Images, logos, favicons
- **robots.txt** — Search engine crawling guidelines
- **sitemap.xml** — XML sitemap for SEO

## Quick Links

- 📧 **Form Integration:** FormSubmit AJAX (appointment requests → configured email)
- 🌐 **Live Site:** https://navira-final-6.vercel.app

## Features

✅ Fully responsive (mobile, tablet, desktop)  
✅ Appointment request form with validation  
✅ Receipt generation & print/WhatsApp sharing  
✅ Smooth animations & transitions  
✅ Accessibility: ARIA labels, keyboard navigation, focus management  
✅ SEO optimized: canonical URL, OG tags, Twitter cards, sitemap  
✅ No backend, database, or authentication required  

## Local Testing

```bash
# Start a local server (Python)
python -m http.server 8000

# Or with Node.js
npx http-server
```

Then visit http://localhost:8000

**Note:** Form submissions show a friendly notification on localhost. They send emails on the live Vercel deployment.

## Sections

- **Home** — Hero, clinic overview
- **About** — Clinic mission, team, community care
- **Services** — Medical services offered
- **Facilities** — Clinic amenities
- **Specialist Care** — Provider network & community programs
- **Contact** — Map, hours, phone, email, WhatsApp
- **Book Appointment** — Appointment request form (FormSubmit AJAX)

## Form Setup

Form submissions use FormSubmit AJAX directly. No account creation, API key, database, or backend server required.

## Tech Stack

- **HTML5** — Semantic, accessible markup
- **CSS3** — No frameworks (pure CSS)
- **JavaScript** — Vanilla JS, no dependencies
- **Forms** — FormSubmit (static form service)
- **Hosting** — Vercel (static site)

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Accessibility

- Semantic HTML structure
- ARIA labels & roles
- Keyboard navigation throughout
- Focus management for modals
- Color contrast WCAG compliant
- Alt text on all images

## Performance

- Single HTML file (no build step)
- Optimized WebP images
- CSS animations (no heavy JS)
- Lazy loading on images
- No external dependencies

## File Size

- `index.html` — ~355 KB
- `assets/` — ~5 MB (images)
- **Total** — ~5.5 MB

---
