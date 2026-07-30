# Tesla Homepage Clone

A front-end recreation of the Tesla.com homepage, built with plain **HTML5** and **CSS3**. This is a practice project focused on layout, typography, and visual fidelity — recreating a real, production-grade marketing site from scratch to sharpen core front-end skills.

> ⚠️ **Disclaimer:** This is an unofficial fan/learning project for educational purposes only. It is not affiliated with, endorsed by, or connected to Tesla, Inc. All Tesla branding, product names, and imagery belong to their respective owners.

---

## 📋 Overview

| | |
|---|---|
| **Project** | `motso-project01-tesla-clone` |
| **Type** | Static front-end clone (HTML/CSS) |
| **Status** | 🚧 In progress — practice build |
| **Live demo** | *Deployed* |

This build recreates the key sections of the Tesla homepage:

- **Header** — logo, primary nav (Vehicles, Energy, Charging, Discover, Shop), and utility icons (help, language, profile)
- **Hero section** — Model 3 promo heading, subheading, and CTA buttons (Order Now / Learn More)
- **Full Self-Driving card** — stat highlights (7x fewer collisions, 11,000+ miles driven) with a looping background video
- **Vehicle carousel** — mini-cards for Model 3, Model Y, and Cybertruck with pricing, CTAs, and dot indicators
- **Footer** — legal/nav links (Privacy & Legal, Vehicle Recalls, Contact, News, etc.)

---

## 🗂️ Project Structure

```
motso-project01-tesla-clone/
├── index.html        # Main page markup
├── styles.css         # All styling
├── images/            # Logos, icons, and vehicle imagery
├── Video/              # Background/promo video assets (e.g. homepage FSD clip)
└── README.md
```

---

## 🛠️ Tech Stack

- **HTML5** — semantic structure, no framework
- **CSS3** — custom styles (no Bootstrap/Tailwind currently in use)
- **No JavaScript yet** — nav, carousel dots, and buttons are currently static markup (see [Known Issues](#-known-issues--next-steps))

---

## 🚀 Getting Started

No build tools or dependencies required — this is a static site.

1. **Clone the repo**
   ```bash
   git clone https://github.com/kgomotsodibetso/motso-project01-tesla-clone.git
   cd motso-project01-tesla-clone
   ```
2. **Open it**
   - Easiest: double-click `index.html` to open it in your browser, **or**
   - Recommended (avoids relative-path/video issues): serve it locally, e.g. with VS Code's **Live Server** extension, or:
     ```bash
     npx serve .
     ```

---

## 🐞 Known Issues / Next Steps

A few things worth cleaning up as this project matures:

- [ ] `index.html` has a duplicate `<html>` opening tag (line 8) — remove the extra one.
- [ ] Several `<div>` tags are missing closing `>` (e.g. around the hero heading and FSD stat block) — these render because browsers are forgiving, but they should be fixed for valid HTML.
- [ ] The vehicle carousel (`.mini-cards` + `.dot-indicators`) is markup-only — dot navigation and slide-switching need JavaScript to actually function.
- [ ] Nav links, "Order Now," and "Learn More" buttons are all placeholder `href="#"` — no routing/pages yet.
- [ ] No responsive/mobile breakpoints confirmed yet — worth testing at common screen widths.
- [ ] Consider adding a `.gitignore` and, if this grows, a `package.json` if tooling (bundler, linter) gets introduced later.

---

## 🎯 Purpose

Built as a hands-on exercise in the transition into software/front-end engineering — practicing pixel-matching a real, complex commercial layout (gradient text, video-backed cards, carousel structure) using only fundamentals before introducing frameworks or JavaScript interactivity.

---

## 📄 License

No license specified — for personal/educational use. Add a `LICENSE` file if you intend to make this reusable by others.
