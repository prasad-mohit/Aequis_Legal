# 🏛️ Amagi Legal — Website

**Advocate Utkarsh Kumar | Supreme Court · Delhi HC · Allahabad HC**

---

## 📁 File Structure

```
website/
├── index.html          ← Main website (all sections)
├── styles.css          ← Full stylesheet
├── script.js           ← Animations, counters, tracking
├── landing-ppc.html    ← Dedicated Google Ads / Meta Ads landing page
├── robots.txt          ← Search engine crawl rules
├── sitemap.xml         ← XML sitemap for Google
└── README.md           ← This file
```

---

## 🚀 Quick Start

1. Upload all files to your web hosting (e.g., Hostinger, GoDaddy, AWS S3).
2. Point your domain `amagılegal.in` (or chosen domain) to the hosting.
3. Enable HTTPS (free via Let's Encrypt or hosting panel).
4. Replace placeholder IDs (see below).

---

## 🔧 Configuration Checklist

### Google Analytics 4 + Google Ads
In `index.html` and `landing-ppc.html`, replace:
- `G-XXXXXXXXXX` → Your **GA4 Measurement ID**
- `AW-XXXXXXXXX` → Your **Google Ads Conversion ID**
- `AW-XXXXXXXXX/XXXXXXXXXX` → Your **Conversion Label** (from Google Ads > Conversions)

### Meta / Facebook Pixel
In `index.html`, replace:
- `YOUR_PIXEL_ID` → Your **Facebook Pixel ID** (from Meta Ads Manager > Events Manager)

### Contact Form Backend
The form currently shows a success message after 1.8s (simulated).
To make it actually send emails, choose one:

**Option A — Formspree (easiest, free):**
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

**Option B — EmailJS (no backend needed):**
1. Sign up at emailjs.com
2. Add their SDK and replace the `handleFormSubmit` function in `script.js`

**Option C — Custom backend (Node.js / PHP)**

---

## 📊 Google Ads Campaign Setup

### Recommended Campaign Structure

**Campaign 1 — Supreme Court / High Court (Search)**
- Keywords: `supreme court advocate delhi`, `high court lawyer delhi`, `advocate supreme court india`
- Landing Page: `landing-ppc.html`

**Campaign 2 — Arbitration (Search)**
- Keywords: `arbitration lawyer india`, `ICC arbitration advocate`, `commercial arbitration delhi`

**Campaign 3 — Corporate Law (Search)**
- Keywords: `corporate lawyer delhi`, `IBC insolvency lawyer`, `NCLT advocate india`

**Campaign 4 — Criminal Defence (Search)**
- Keywords: `criminal lawyer supreme court`, `bail advocate delhi`, `criminal defence advocate`

**Campaign 5 — Remarketing (Display)**
- Target: website visitors who didn't convert
- Ad: "Still need legal help? Book your FREE consultation today."

### Conversion Actions to Set Up in Google Ads
1. **Form Submit** → Thank you page view OR form submit event
2. **Phone Call** → Click on phone number link (use Call Extensions too!)
3. **WhatsApp Click** → Custom event `whatsapp_click`

---

## 📱 Meta Ads Campaign Setup

**Audience Targeting:**
- Location: Delhi NCR, Lucknow, Mumbai, Bangalore
- Age: 28–65
- Interests: Legal services, Business law, Litigation, Arbitration, Real estate
- Behaviours: Business owners, High-income households

**Custom Events Tracked:**
- `Lead` → Form submission
- `Contact` → Phone click / WhatsApp click

**Recommended Ad Formats:**
- Lead Generation Ads (instant form — highest conversion for legal)
- Traffic Ads → `landing-ppc.html`
- Video Ads (record a 30-sec intro by Adv. Utkarsh)

---

## 🔍 SEO Checklist

- [ ] Replace `amagılegal.in` with actual domain in `index.html`, `sitemap.xml`, `robots.txt`
- [ ] Add actual `og-image.jpg` (1200×630px) — professional photo of advocate/office
- [ ] Register on **Google Business Profile** (free local SEO)
- [ ] Submit sitemap.xml to Google Search Console
- [ ] Add to **Justdial**, **Sulekha**, **Lawyered**, **LegalKart** directories

---

## 🎨 Design Notes

- **Color Palette:** Deep Navy (#0B1D3A), Legal Gold (#C9A84C), Crimson (#8B1A1A)
- **Fonts:** Cinzel (headings, logo), Inter (body), Playfair Display (accent)
- **Style:** Premium Indian legal aesthetic — gravitas + modernity
- **Hero BG:** Unsplash — Indian court / scales of justice imagery

---

## 📞 Contact Details (Pre-filled)

| Field | Value |
|-------|-------|
| Advocate | Utkarsh Kumar |
| Phone 1 | +91-8948-268-809 |
| Phone 2 | +91-8318-596-409 |
| Email | utk.adv2103@gmail.com |
| Office | 80, Second Floor, Golf Links, New Delhi – 110 003 |
| Education | RMLNLU Lucknow, B.A. LL.B (Hons.) 2021 |

---

*Built for Amagi Legal · 2025*
