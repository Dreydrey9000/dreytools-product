# dreytools-product

Product page for **Drey Playbook** — a real digital-product landing that can live at dreythomas.com when Stripe is wired.

**Live:** https://product.dreytools.com
**CF project:** `dreytools-product`

## What it has

- Sticky nav with brand pulse dot + Buy CTA
- Hero: eyebrow badge, hero headline, trust row (stars + count + refund), buy card with price/old-price/save badge, main CTA
- Animated product cover (rotates on hover) — self-drawn in CSS, no image needed
- Features strip (3 inline feature chips)
- "What's inside" 9-module curriculum
- 3 testimonials with colored initial avatars
- FAQ (5 accordion items)
- Final CTA section
- Warm dark + cyan brand
- Mobile-first responsive

## Checkout flow

Currently routes the Buy button to `contact.dreytools.com?topic=Hire` as a fallback while Stripe is pending. Swap the JS `window.location.href` for a real Stripe Checkout Session when keys are live.

## Stack

Pure HTML + CSS + vanilla JS. Single file. Zero dependencies.

## Deploy

```bash
wrangler pages deploy . --project-name dreytools-product --branch main
```
