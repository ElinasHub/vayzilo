# Vayzilo — Airbnb Alternative

A modern, fully responsive website for **Vayzilo.com**, built as a clean alternative to Airbnb.

## Features

- Beautiful landing page with hero search
- Category filters (Beach, Mountain, City, Unique, Luxury)
- Search by location and guest count
- Listing cards with high-quality images
- Detailed property modal with booking request form
- Auth modals (demo)
- Host CTA section
- Mobile-responsive design
- Zero external dependencies beyond Tailwind CDN & Google Fonts

## Branding

- Primary color: Teal (`#0F766E`)
- Accent: Amber
- Tagline: "Stay unique. Book direct."
- Positioning: Lower fees (5% host / 0% guest), verified hosts, unique stays

## How to deploy to vayzilo.com

1. Upload the contents of this folder to any static host:
   - **Netlify**: Drag & drop the folder
   - **Vercel**: `vercel` CLI or connect GitHub
   - **GitHub Pages**: Push to a repo and enable Pages
   - **Your own server**: Copy `index.html` to the web root

2. Point your domain `vayzilo.com` to the host.

That's it — it's a single `index.html` file. No build step required.

## Next steps for a full product

- Connect a real backend (Supabase, Firebase, or custom API)
- Add user authentication
- Implement real booking & payments (Stripe)
- Host dashboard for listing management
- Reviews, messaging, calendar availability
- Image upload for hosts

Enjoy your new platform!
