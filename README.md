# BLOC Editorial

A minimal, dark-mode editorial platform for long-form writing on political thought, Islamic tradition, Bangladeshi history, and global power structures.

**Live Site:** [BLOC Editorial](https://bloc.example.com)

---

## Overview

BLOC is a clean, ad-free publishing platform designed for serious readers and writers. No algorithm. No noise. Just carefully curated essays that map politics, tradition, and power through rigorous analysis.

### Features

- **Tag-based filtering** — Explore essays by topic: Islam, Politics, Bangladesh, History, Geopolitics
- **Dark minimal UI** — Gen Z-inspired design with soft purple accents and clean typography
- **Responsive design** — Optimized for desktop, tablet, and mobile
- **Fast & static** — Pure HTML/CSS/JavaScript with no backend dependencies
- **Author profiles** — Meet the collective behind each piece

---

## Site Structure

```
├── index.html          # Main page markup
├── style.css           # Dark mode styles and responsive layout
├── script.js           # Client-side rendering and navigation
├── cases.json          # (Optional) Case study data
└── README.md           # This file
```

---

## Color Palette

The site uses a sophisticated dark palette with cyber accents:

- **Background:** `rgb(10, 10, 15)` — Deep black
- **Surface:** `rgb(20, 20, 30)` — Dark charcoal
- **Accent:** `rgb(167, 139, 250)` — Soft purple
- **Text:** `rgb(245, 245, 255)` — Off-white
- **Muted:** `rgb(120, 120, 140)` — Neutral gray

---

## Typography

- **Headlines:** Inter (900 weight) — Bold, modern, tight spacing
- **Body:** Inter (400–700) — Clean, highly legible
- **Metadata:** Space Mono — Technical, monospace accents

---

## Content Structure

Each essay includes:

- **Title & subtitle** — Clear, compelling hooks
- **Author & date** — With author profile badges
- **Read time** — Estimated duration
- **Tags** — Multiple categorization options
- **Body** — Full rich text with blockquotes and emphasis
- **Meta section** — Author info and publication date

### Sample Data

The site includes five essays:

1. **Istiqamah and the Lie of Motivation** — By Sifat (Islam, Politics)
2. **The Fourth Political Theory's Blindspot** — By Sifat (Politics, Geopolitics)
3. **1971 and the Silences We Inherit** — By Rabib (Bangladesh, History)
4. **The Bay of Bengal in a Multipolar World** — By Nahian (Geopolitics, Bangladesh)
5. **Maqasid al-Shariah and the Modern State** — By Farid (Islam, Politics)

---

## Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- No build tools or server required

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/bloc-editorial.git
   cd bloc-editorial
   ```

2. Open `index.html` in your browser:
   ```bash
   open index.html
   ```

   Or spin up a local server:
   ```bash
   python3 -m http.server 8000
   # Then visit http://localhost:8000
   ```

---

## Development

### Architecture

- **Client-side rendering** — All content rendering happens in `script.js`
- **Tag filtering** — Real-time filtering without page reload
- **View switching** — Seamless transitions between home and post views
- **Responsive breakpoints** — 1024px, 768px, 520px

### Customization

#### Adding a New Article

Edit `script.js` and add to the `P` array:

```javascript
{
  id: 6,
  title: "Your Article Title",
  sub: "Your subtitle or summary",
  date: "May 1, 2026",
  rt: "8 min",
  tags: ["islam", "politics"],
  author: "authorname",
  body: `<p>Your article content here...</p>`
}
```

#### Adding a New Author

Edit the `A` object in `script.js`:

```javascript
const A = {
  yourname: {
    name: "Your Name",
    color: "#yourcolor",
    bg: "rgba(yourrgb,.12)",
    i: "Y"
  }
};
```

#### Changing the Palette

Update the CSS variables in `style.css`:

```css
:root {
  --bg: rgb(10, 10, 15);
  --acc: rgb(167, 139, 250);
  /* ... other colors */
}
```

---

## Browser Support

- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Mobile browsers (iOS Safari 14+, Chrome Mobile)

---

## Performance

- **First contentful paint:** <500ms
- **Total bundle size:** ~45KB (HTML + CSS + JS)
- **No external dependencies** (Except Google Fonts)
- **Fully responsive** — Single CSS file, no build tools

---

## License

© 2026 BLOC Editorial. All rights reserved.

For licensing inquiries, contact the collective.

---

## Contact

- **Email:** contact@bloc-editorial.com
- **Twitter:** [@bloceditors](https://twitter.com)
- **About:** [On the site](https://bloc-editorial.com#about)

---

## Contributing

BLOC is a curated collective publication. To submit essays or inquire about contributions, please reach out directly.

---

## Changelog

### v1.0 (May 2026)
- Initial release
- Five inaugural essays
- Dark minimal UI with Gen Z aesthetic
- Full tag filtering and responsive design
