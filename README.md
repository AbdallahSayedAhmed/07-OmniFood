# 🍽️ Omnifood

> A healthy meal delivered to your door, every single day.

**Omnifood** is a responsive, AI-themed food subscription landing page built as part of the *"Build Responsive Real-World Websites with HTML and CSS"* course. The site markets a fictional service that generates personalized weekly meal plans and delivers them daily, 365 days a year.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

---

## 📖 Overview

Omnifood positions itself as a technology-first company focused on consumer well-being. Users select their dietary preferences and restrictions, an AI algorithm builds a custom weekly meal plan, and local cooking partners prepare and deliver the meals — all under a simple monthly subscription.

This project recreates the full marketing site: hero section, features, pricing, testimonials, photo gallery, and a signup call-to-action, built with **semantic HTML**, **modern CSS** (custom properties, Flexbox, CSS Grid), and a touch of **vanilla JavaScript** for interactivity.

## ✨ Features

- **Responsive layout** — adapts across desktop, tablet, and mobile breakpoints
- **Sticky navigation** — header becomes sticky on scroll using the `IntersectionObserver` API
- **Smooth scrolling** — animated in-page navigation for all anchor links, with a polyfill for broader browser support
- **Dynamic copyright year** — footer year updates automatically via JavaScript
- **Cross-browser fallback** — feature-detects the CSS `gap` property in Flexbox and applies a margin-based fallback for older Safari versions
- **PWA-ready manifest** — includes a `manifest.webmanifest` with app icons
- **Signup form** — CTA form wired to [Formspree](https://formspree.io/) for submission handling
- **Accessible markup** — descriptive `alt` text, semantic sectioning, and icon labeling via [Ionicons](https://ionic.io/ionicons)

## 🧩 Sections

| # | Section | Description |
|---|---------|--------------|
| 1 | Navigation | Logo + anchor links to all major sections |
| 2 | Hero | Headline, CTA buttons, and social proof (customer avatars) |
| 3 | Featured In | Press/media logos strip |
| 4 | How It Works | 3-step explainer with app screenshots |
| 5 | Meals & Diets | Sample meal cards and supported diet types |
| 6 | Testimonials & Gallery | Customer quotes and a 12-photo food gallery |
| 7 | Pricing & Features | Two subscription tiers and 4 key benefits |
| 8 | CTA | Free first-meal signup form |
| 9 | Footer | Contact info, social links, and site navigation |

## 🛠️ Tech Stack

- **HTML5** — semantic structure
- **CSS3** — custom properties (design tokens), Flexbox, CSS Grid, responsive media queries
- **JavaScript (ES6+)** — DOM interaction, `IntersectionObserver`, feature detection
- **[Ionicons](https://ionic.io/ionicons)** — icon set (loaded via CDN as ES modules)
- **[Google Fonts](https://fonts.google.com/)** — Rubik typeface
- **[Formspree](https://formspree.io/)** — form backend for the signup CTA
- **[smoothscroll-polyfill](https://github.com/iamdustan/smoothscroll-polyfill)** — smooth-scroll support for Safari

## 📁 Project Structure

```
07-OmniFood/
├── index.html              # Main page markup
├── content.md               # Source copy & content reference (gitignored)
├── manifest.webmanifest    # PWA manifest & app icons
├── CSS/
│   ├── general.css         # Design tokens, resets, and base/global styles
│   ├── style.css           # Component & section-specific styles
│   └── queries.css         # Flexbox-gap fallback rules for older Safari
├── JS/
│   └── script.js           # Sticky nav, smooth scroll, dynamic year, feature detection
└── img/
    ├── app/                # App screenshots (3)
    ├── customers/           # Customer avatars & testimonial photos (10)
    ├── gallery/              # Food gallery photos (12)
    ├── logos/                # Featured-in press logos (5)
    ├── meals/                # Sample meal photos (2)
    └── *.png                # Hero image, site logo, and favicons
```

## 🎨 Design System

Defined at the top of `CSS/general.css`:

- **Primary color:** `#e67e22` (with tint/shade scale for hover and background states)
- **Typography:** Rubik font family, sizes on a 10–98px scale, base `1rem = 10px`
- **Spacing scale:** 2 / 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64 / 80 / 96 / 128 (px)
- **Border radius:** `0.9rem` default
- **Grid system:** custom `.grid` utility classes (`grid--2-cols`, `grid--3-cols`, `grid--4-cols`, `grid--footer`)

## 🚀 Getting Started

No build tools or dependencies required — this is a static site.

1. **Clone the repository**
   ```bash
   git clone https://github.com/AbdallahSayedAhmed/07-OmniFood.git
   cd 07-OmniFood
   ```
2. **Open `index.html`** directly in a browser, or serve it locally for the best experience (e.g. with the VS Code *Live Server* extension) so relative asset paths resolve correctly.

## 🌐 Browser Support

Tested with fallbacks for older Safari versions (Flexbox `gap` polyfill and a smooth-scroll polyfill). Best viewed in a modern evergreen browser (Chrome, Edge, Firefox, Safari).

## 📝 Notes

- `content.md` holds the original copy/content brief used to build the page and is excluded from version control via `.gitignore`.
- The mobile hamburger navigation and a few interactive scripts are present in `JS/script.js` but currently commented out — left as an open exercise from the course.
- Footer social links, account links, and "See all recipes" are placeholder anchors (`#`) with no real destinations yet.

## 🙏 Credits

- Built as part of the Udemy course **["Build Responsive Real-World Websites with HTML and CSS"](https://www.udemy.com/)** by Jonas Schmedtmann.
- Design, copywriting, and image assets (meals, gallery, customer photos, app mockups) are provided as course material for educational purposes.

## 📄 License

This project is for educational/portfolio purposes. Course-provided design and image assets remain the property of their original creators.

---

**Author:** Abdallah Sayed Ahmed · [GitHub](https://github.com/AbdallahSayedAhmed)
