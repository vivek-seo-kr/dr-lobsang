# Dolma Memorial Clinic — Website

A single-page website for **Dolma Memorial Clinic**, a Traditional Tibetan Medicine (Sowa Rigpa) practice located in McLeod Ganj, Dharamshala. The site is built as a self-contained HTML file with no build step or dependencies required.

---

## Overview

The website presents the clinic's heritage, services, gallery, patient testimonials, FAQs, and a contact/inquiry section. It honours the legacy of **Dr. Lobsang Dolma Khangkar** — the first woman physician in the Tibetan Sowa Rigpa tradition.

---

## Tech Stack

| Technology | Purpose |
|---|---|
| HTML5 | Page structure |
| [Tailwind CSS](https://tailwindcss.com/) (CDN) | Utility-first styling |
| [Alpine.js](https://alpinejs.dev/) (CDN) | Lightweight interactivity (mobile menu, FAQ accordion, scroll behaviour) |
| [Lucide Icons](https://lucide.dev/) (CDN) | Icon set |
| Google Fonts — Inter | Typography |

No build tools, bundlers, or package managers are needed.

---

## File Structure

```
portfolio.html    # The entire website in a single file
README.md         # This file
```

---

## Sections

| Section | Anchor | Description |
|---|---|---|
| Hero | `#home` | Headline, stats (4.8 rating, 40+ years, 10k+ patients), and CTA buttons |
| Why Choose Us | — | Four feature cards: Expert Doctors, Authentic Medicine, Holistic Approach, Patient Centric |
| Services | `#services` | Pulse Diagnosis, Herbal Remedies, Dietary Guidance |
| About | `#about` | Clinic legacy and Dr. Lobsang Dolma Khangkar's story |
| Gallery | `#gallery` | Visual tour of the clinic |
| FAQs | `#faqs` | Accordion-style frequently asked questions |
| Testimonials | — | Patient reviews |
| Contact | `#contact` | Address, phone, hours, and an inquiry form |
| Footer | — | Navigation links, Privacy Policy, Terms of Service |

---

## Running the Website

Because the site is a single HTML file with all dependencies loaded from CDNs, no installation is required.

1. Open `portfolio.html` directly in any modern web browser.
2. Alternatively, serve it with any static file server for local development:

```bash
# Python
python -m http.server 8080

# Node.js (npx)
npx serve .
```

Then visit `http://localhost:8080/portfolio.html`.

---

## Customisation

All content is contained within `portfolio.html`. Key areas to update:

- **Clinic name & tagline** — `<title>` tag and the `<nav>` logo block.
- **Contact details** — Phone number (`075900 32466`), address (`Dolma Chowk, McLeod Ganj`), and opening hours appear in the top bar and the contact section.
- **Hero stats** — Rating, years of legacy, and patient count are hardcoded in the hero section.
- **Colour theme** — Custom colours are defined in the `tailwind.config` script block at the top of the file under the `medical` key.
- **Images** — Hero and gallery images are currently loaded from external URLs; replace with local paths as needed.
- **Services** — Add or remove service cards inside `<section id="services">`.

---

## Browser Support

The site targets all modern evergreen browsers (Chrome, Firefox, Safari, Edge). It does not support Internet Explorer.

---

## Contact

**Dolma Memorial Clinic**  
Dolma Chowk, McLeod Ganj, Dharamshala  
📞 075900 32466  
🕐 Monday – Saturday: 9:00 AM – 5:00 PM
