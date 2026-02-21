# Tierra y Tinta — Website Development Plan

## Overview
Custom art jewelry site for **Tierra y Tinta**: real-orchid earrings and necklaces, slow-crafted in Miami. Low inventory → purchase page shows “out of stock” message and collects name/email for restock contact.

---

## 1. Design System (from business cards)

| Element | Choice |
|--------|--------|
| **Background** | Warm aged beige / off-white (`#f5f0e8`, `#ebe5d9`) with subtle paper texture |
| **Accent / text** | Deep plum / purple (`#4a3f6b`, `#5c4d7a`) for headings, links, buttons, borders |
| **Headings** | Serif (e.g. **Libre Baskerville**, **Cormorant Garamond**) — “THANK YOU” / “Tierra y Tinta” style |
| **Body / UI** | Clean sans-serif (e.g. **Source Sans 3**, **Karla**) |
| **Slogan / tagline** | Italic serif or script (e.g. **Dancing Script**, **Cormorant Italic**) — “Slow crafted in Miami, Florida” |
| **Motif** | Orchid + “TT” monogram (stamp) — use as favicon, section accent, or small logo |
| **Vibe** | Vintage postcard, artisanal, personal, elegant |

---

## 2. Site Structure

```
/
├── index.html          # Front page
├── about.html          # About Us
├── purchase.html       # Shop / Purchase (out-of-stock + notify form)
├── css/
│   └── styles.css      # Global styles, variables, layout
└── assets/             # Optional: logo, texture, favicon
```

---

## 3. Page Specifications

### 3.1 Front Page (`index.html`)
- **Header**: Sticky or static nav — Home, About Us, Purchase.
- **Hero**: Large “Tierra y Tinta”, tagline “Slow crafted in Miami, Florida”, optional orchid/paper texture.
- **Intro**: Short line about real-orchid jewelry (earrings & necklaces).
- **Instagram**: “Follow us” + link to [@tierraytinta.mia](https://instagram.com/tierraytinta.mia), optional QR or icon.
- **Footer**: Slogan, Instagram, copyright.

### 3.2 About Us (`about.html`)
- **Story**: How jewelry is made from real orchids; custom, artisanal, Miami.
- **Values**: Slow crafted, quality, personal touch (“To: Beloved Customer” tone).
- **Slogan**: “Slow crafted in Miami, Florida” prominent.
- **Contact / follow**: Instagram @tierraytinta.mia, optional “Get notified” link to purchase page.

### 3.3 Purchase Page (`purchase.html`)
- **Main message**:  
  “Sorry we ran out of inventory. Please leave your name and email and we will contact you when we have more inventory.”
- **Form**: Name (required), Email (required), Submit.
- **Behavior**: On submit, show thank-you message (no backend required for MVP; form can be `mailto:` or placeholder for future backend).
- **Same header/footer** as rest of site.

---

## 4. Content Checklist
- [ ] Brand name: Tierra y Tinta
- [ ] Tagline: Slow crafted in Miami, Florida
- [ ] Instagram: @tierraytinta.mia
- [ ] Product focus: real orchid jewelry — earrings, necklaces
- [ ] Out-of-stock copy and notify form on purchase page

---

## 5. Technical Notes
- **Fonts**: Google Fonts (Libre Baskerville or Cormorant + Source Sans 3 + Dancing Script or Cormorant Italic).
- **Responsive**: Mobile-first; nav can collapse to hamburger on small screens.
- **Form**: Name + email + “Notify me” button; optional `action="#"` and `onsubmit` thank-you for now; later connect to Formspree, Netlify Forms, or custom backend.
- **Texture**: Optional CSS `background-image` with a subtle paper texture or very light noise.

---

## 6. Next Steps (after this build)
1. Add backend or form service for notify-me submissions.
2. Add real product photos and an inventory system when stock returns.
3. Optional: Instagram embed or gallery.
4. Favicon: orchid or “TT” from stamp design.
