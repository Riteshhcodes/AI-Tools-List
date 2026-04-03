# ⬡ AI Design Tools Universe

> **The most complete directory of AI-powered design tools — curated, rated & reviewed.**
> 30+ tools across 8 categories, with ratings, quality scores, pros/cons, and direct links.

![Version](https://img.shields.io/badge/version-1.0.0-6c63ff?style=flat-square)
![Tools](https://img.shields.io/badge/tools-30%2B-ff6b9d?style=flat-square)
![React](https://img.shields.io/badge/React-18.2-61dafb?style=flat-square&logo=react)
![License](https://img.shields.io/badge/license-MIT-00d4aa?style=flat-square)

---

## 🌐 Live Demo

**[👉 View Live Site](https://yourusername.github.io/ai-design-tools)**

---

## 📸 Preview

```
┌─────────────────────────────────────────────┐
│  ⬡ AI Design Universe          ★ GitHub     │
├─────────────────────────────────────────────┤
│                                             │
│     The Ultimate AI Design Tools           │
│              Universe                       │
│                                             │
│  30+ Tools  ·  8 Categories  ·  4.3★ Avg   │
│                                             │
│  [ 🔍 Search tools... ]                    │
│                                             │
│  [All] [UI/UX] [Image Gen] [Motion] [3D]   │
│                                             │
│  ┌──────────┐ ┌──────────┐ ┌──────────┐   │
│  │ 🎨 Figma │ │ 🔥 Adobe │ │ ⚡Framer │   │
│  │  4.9 ★  │ │  4.6 ★  │ │  4.7 ★  │   │
│  └──────────┘ └──────────┘ └──────────┘   │
└─────────────────────────────────────────────┘
```

---

## ✨ Features

- 🔍 **Live Search** — Search by tool name, category, or use case
- 🏷️ **Filter by Category** — UI/UX, Image Gen, Prototyping, Motion, 3D, Color, Wireframing, Design Systems
- 💰 **Filter by Pricing** — Free, Freemium, Paid, Open Source
- ⭐ **Ratings & Quality Scores** — Community ratings + curated quality percentages
- ✅ **Pros & Cons** — Toggle per tool to see detailed breakdowns
- 🚀 **Featured Tools** — Highlighted top picks across categories
- 📱 **Fully Responsive** — Works on mobile, tablet, and desktop
- 🌙 **Dark Theme** — Beautiful dark UI throughout

---

## 🗂️ Categories Covered

| Category | Tools Included |
|---|---|
| 🎨 UI/UX Design | Figma, Penpot, Galileo AI, Framer, Dora AI... |
| 🖼️ Image Generation | Midjourney, Adobe Firefly, Stable Diffusion, Canva AI, Krea AI... |
| ⚡ Prototyping | Framer, Protopie, Maze, Beautiful.ai... |
| 🌀 Motion | Rive, Runway ML, LottieFiles, Pika Labs... |
| 🔮 3D & Spatial | Spline, Luma AI, Blockade Labs... |
| 🖊️ Wireframing | Uizard, Visily, Whimsical, Autodraw... |
| 🧩 Design Systems | Relume, Locofy.ai, Diagram/Genius, Uxcel... |
| 🌈 Color Tools | Khroma, Coolors, Fontjoy... |

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Framework | React 18 |
| Styling | CSS-in-JS (inline styles) + Google Fonts |
| Data | Static JS module (`src/data/tools.js`) |
| Fonts | Syne (display) + DM Sans (body) |
| Hosting | GitHub Pages |
| Build | Create React App |

---

## 🚀 Getting Started

### Prerequisites

Make sure you have these installed:
- [Node.js](https://nodejs.org/) v16 or higher
- npm (comes with Node.js)

Check your versions:
```bash
node --version
npm --version
```

### Installation

**1. Clone the repository**
```bash
git clone https://github.com/yourusername/ai-design-tools.git
cd ai-design-tools
```

**2. Install dependencies**
```bash
npm install
```

**3. Start the development server**
```bash
npm start
```

Open [http://localhost:3000](http://localhost:3000) in your browser. The page reloads automatically when you make changes.

---

## 📦 Build for Production

```bash
npm run build
```

This creates an optimized production build in the `build/` folder, ready to deploy.

---

## 🌍 Deploy to GitHub Pages

**Step 1 — Install gh-pages**
```bash
npm install --save-dev gh-pages
```

**Step 2 — Add to `package.json`**
```json
{
  "homepage": "https://yourusername.github.io/ai-design-tools",
  "scripts": {
    "predeploy": "npm run build",
    "deploy": "gh-pages -d build"
  }
}
```

**Step 3 — Deploy**
```bash
npm run deploy
```

Your site will be live at `https://yourusername.github.io/ai-design-tools` 🎉

---

## 📁 Project Structure

```
ai-design-tools/
│
├── public/
│   └── index.html              # HTML entry point
│
├── src/
│   ├── components/
│   │   ├── Navbar.jsx          # Sticky navigation bar
│   │   ├── Hero.jsx            # Hero section with stats
│   │   ├── FilterBar.jsx       # Search + category filters
│   │   ├── ToolCard.jsx        # Individual tool card
│   │   └── Footer.jsx          # Footer section
│   │
│   ├── data/
│   │   └── tools.js            # All tool data (name, rating, desc, etc.)
│   │
│   ├── styles/
│   │   └── App.css             # Global styles + CSS variables
│   │
│   └── App.jsx                 # Root component + filter logic
│
├── package.json
└── README.md
```

---

## ➕ Adding a New Tool

Open `src/data/tools.js` and add an entry to the `tools` array:

```js
{
  id: 31,                                         // unique number
  name: "Tool Name",
  type: "UI/UX Design",                          // primary category
  icon: "🛠",                                     // emoji icon
  iconBg: "linear-gradient(135deg,#color1,#color2)",
  rating: 4.5,                                   // out of 5
  users: "500K+",
  desc: "Short description of what the tool does and its AI features.",
  pricing: "freemium",                           // "free" | "paid" | "freemium"
  quality: 88,                                   // 0–100 quality score
  featured: false,                               // true to show Featured badge
  openSource: false,                             // true for open-source tools
  tags: ["UI/UX Design", "Prototyping"],         // filter categories
  url: "https://tool-website.com",
  pros: ["Pro one", "Pro two", "Pro three"],
  cons: ["Con one", "Con two"],
  founded: 2022,
  platform: ["Web", "Desktop"],
},
```

Save the file — the tool will appear instantly in the grid.

---

## 🎨 Customization

### Change the color theme
Edit CSS variables in `src/styles/App.css`:
```css
:root {
  --accent: #6c63ff;    /* primary purple */
  --accent2: #ff6b9d;   /* pink accent */
  --accent3: #00d4aa;   /* teal accent */
  --bg: #0a0a0f;        /* page background */
  --card: #16161f;      /* card background */
}
```

### Change fonts
Replace the Google Fonts import in `App.css` and update `--font-display` / `--font-body` variables.

---

## 🤝 Contributing

Contributions are welcome! If you know an AI design tool that should be listed:

1. Fork the repository
2. Create a new branch: `git checkout -b add-tool-name`
3. Add the tool to `src/data/tools.js`
4. Commit: `git commit -m "Add ToolName to directory"`
5. Push: `git push origin add-tool-name`
6. Open a Pull Request

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgements

- Tool data sourced from official websites and community reviews
- Fonts by [Google Fonts](https://fonts.google.com) — Syne & DM Sans
- Built with [Create React App](https://create-react-app.dev)
- Deployed via [GitHub Pages](https://pages.github.com)

---

<div align="center">
  <strong>⬡ AI Design Universe</strong> · Made with ❤️ · 2025
</div>
