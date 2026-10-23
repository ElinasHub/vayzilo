# Vayzilo — Vacation Rentals. Reimagined for the AI Era.

The website for **Vayzilo.com**, an emerging vacation rental marketplace designed around zero platform commissions, transparent pricing, independent hosts, and future AI-powered travel discovery.

**Status: early development.** The public homepage is a launch page — hero, benefits, AI vision, a Founding Host interest form, and a Traveler Early Access waitlist. Bookings are not yet available.

## What's in the page

- Launch hero ("Vacation Rentals. Reimagined for the AI Era.") with Founding Host + Traveler Waitlist CTAs
- "A Better Way to Stay" benefit cards (hosts / travelers / AI discovery)
- AI discovery vision section (integrations are planned, not yet available)
- Founding Host interest form and Traveler waitlist form (see form capture note below)
- Privacy notice modal
- Mobile-first, responsive, Tailwind via CDN + Google Fonts — still a single `index.html`, no build step

## Preserved marketplace components

The original marketplace shell code — search, category filters, listing cards, property detail modal, auth modals, and demonstration listing data — is preserved in `index.html` for future development. It is **not displayed** on the public homepage: demo properties, prices, ratings, and reviews must never be presented publicly as real.

## Form capture

Registrations are open: both forms POST to FormSubmit's AJAX endpoint, which emails each submission to Elina (subject lines: "Vayzilo — Founding Host registration" / "Vayzilo — Traveler waitlist signup"). FormSubmit requires a one-time activation click in the email it sends on the first submission. If volume ever justifies it, swap `FORM_ENDPOINT` in `index.html` for a real database-backed capture.

## Branding

- Primary: deep teal `#0D716B` (dark variant `#0A5954`)
- Background: warm off-white `#FAF9F6`
- Text: charcoal `#20272A`
- Accent: amber `#F59E0B`
- Positioning: **zero Vayzilo platform commissions** (not "fee-free" overall — payment processing and disclosed third-party costs still apply), transparent pricing, independent hosts, AI-powered discovery

## Deployment

Live via **GitHub Pages** from this repo (`main` branch, root), custom domain `vayzilo.com` (see the `CNAME` file). Push to `main` to deploy. DNS is at GoDaddy: apex A records point to GitHub Pages, `www` CNAME points to `elinashub.github.io`.

## Next steps for a full product

- Connect a real backend (Supabase, Firebase, or custom API)
- Add user authentication
- Implement real booking & payments (Stripe)
- Host dashboard for listing management
- Reviews, messaging, calendar availability
- Image upload for hosts
