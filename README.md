# WA Agent — Website

A clean, single-page website for a **WhatsApp agent service**. We build and manage
WhatsApp agents for businesses: the visitor opens the site, taps one button, and lands
straight in WhatsApp to talk to us. No sign up, no login.

## What is in this repo

| File | Purpose |
|------|---------|
| `index.html` | The website. One self-contained file (HTML, CSS and JS inside). |
| `docs/Startup_Ideas_India_2026.pdf` | Startup ideas research report. |
| `docs/WhatsApp_Agent_30_Day_Plan.pdf` | The 30-day launch plan for this business. |
| `README.md` | This file. |

## Before you go live

1. **Set your WhatsApp number.** Open `index.html`, find the line near the bottom:

   ```js
   var WHATSAPP_NUMBER = "919999999999";
   ```

   Replace it with your real number. Use the country code and digits only, no `+`
   and no spaces. For an Indian number `98123 45678`, write `919812345678`.

2. **Update the placeholders.** Search `index.html` for:
   - `https://your-domain.com/` — put your real website address (used by search engines).
   - The brand name `WA Agent` — change it to your business name.
   - The pricing numbers (`Rs 2,499`, `Rs 9,999`) — set your own.
   - The text in the FAQ and "Why us" sections — make it match your service.

## How to host it

The file is fully static, so any static host works. Pick one:

- **GitHub Pages** — free. In the repository, go to Settings, then Pages, and set the
  source to the `main` branch and the root folder. Your site goes live in a minute.
- **Netlify** or **Cloudflare Pages** — drag and drop the folder, or connect the repo.

## Built for search engines (SEO)

The page already includes:

- A descriptive title and meta description.
- Open Graph and Twitter card tags for clean link previews.
- A canonical URL tag.
- Structured data (JSON-LD) describing the business.
- Semantic HTML with a single main heading and proper section headings.
- Mobile-first responsive layout.

To finish SEO properly, add a share image: create a `1200x630` image, save it as
`og-image.jpg` in this repo, and add this line inside the `<head>` of `index.html`:

```html
<meta property="og:image" content="https://your-domain.com/og-image.jpg" />
```

## Editing the design

Everything is plain HTML and CSS inside `index.html`. There is no build step and no
dependencies. Change the colours in the `:root` block at the top of the `<style>` tag.

## License

Private. All rights reserved.
