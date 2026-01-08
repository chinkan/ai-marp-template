# 📊 AI-Powered Marp Presentation Template

![GitHub license](https://img.shields.io/github/license/chinkan/ai-marp-template)
![Marp](https://img.shields.io/badge/Marp-Ready-0288D1)
![Cursor](https://img.shields.io/badge/Cursor-AI_Powered-black)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

> **Create beautiful slide decks in seconds using Markdown and AI.**  
> This template combines the power of [Marp](https://marp.app/) with custom Cursor AI rules to automate presentation generation.

---

## 🚀 Features

- **🤖 AI Integration**: Built-in Cursor rules to generate, update, and format slides via chat.
- **🎨 Custom Themes**: Includes 5 professionally designed themes (Corporate, Developer, Gradient, Minimal, Midnight).
- **📐 Responsive Layouts**: Support for 16:9, 4:3, and split-screen layouts.
- **🛠️ Developer Ready**: CSS-based styling, hot-reloading dev server, and PDF/PPTX export.
- **📦 Zero Config**: Ready to use immediately with `pnpm` or `npm`.

## 🏁 Quick Start

1. **Use this Template**:
   Click the **[Use this template](https://github.com/new?template_name=ai-marp-template&template_owner=chinkan)** button at the top of the repo to create your own repository.

2. **Clone & Install**:
   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
   pnpm install # or npm install
   ```

3. **Run Dev Server**:
   ```bash
   pnpm dev
   ```
   Open `http://localhost:8080` to see your slides.

## 🤖 AI Commands (Cursor)

This template includes a `.cursor/rules` file that supercharges your workflow. Open `Chat` (Ctrl/Cmd+L) and use these commands:

| Command | Action | Example |
|---------|--------|---------|
| `@slide` | Create a **NEW** presentation from scratch | `@slide Topic: Quarterly Review. Points: Q1 growth, Q2 goals...` |
| `@slide-update` | Modify the **CURRENT** slide deck | `@slide-update Add a slide about "Risks" after the timeline` |
| `@theme` | List and preview available themes | `@theme Show me the midnight theme` |
| `@slide-export` | Export slides to PDF or PPTX | `@slide-export as PDF` |

## 🎨 Themes

All themes are located in `src/themes/` and can be applied globally in the front-matter.

### 1. Corporate (`theme: corporate`)
*Professional, blue-accented theme perfect for business.*
![Corporate Theme Preview](https://via.placeholder.com/600x337/f8f9fa/0056b3?text=Corporate+Theme)

### 2. Developer (`theme: developer`)
*Dark mode with syntax highlighting support.*
![Developer Theme Preview](https://via.placeholder.com/600x337/1e1e1e/569cd6?text=Developer+Theme)

### 3. Gradient (`theme: gradient`)
*Modern, vibrant gradients for high-impact talks.*
![Gradient Theme Preview](https://via.placeholder.com/600x337/fad0c4/ff6b6b?text=Gradient+Theme)

### 4. Minimal (`theme: minimal`)
*Clean, whitespace-heavy design for clarity.*
![Minimal Theme Preview](https://via.placeholder.com/600x337/ffffff/333333?text=Minimal+Theme)

### 5. Midnight (`theme: midnight`)
*Elegant deep navy and gold for evening events.*
![Midnight Theme Preview](https://via.placeholder.com/600x337/0f172a/fbbf24?text=Midnight+Theme)

## 📁 Directory Structure

```
.
├── .cursor/rules/      # 🧠 AI instruction rules
├── src/
│   ├── slides/         # 📝 Your presentation files (.md)
│   ├── themes/         # 🎨 CSS theme definitions
│   ├── demo/           # 👁️ Theme showcases
│   └── assets/         # 🖼️ Images and static assets
├── dist/               # 📦 Build output
└── package.json        # ⚙️ Scripts and dependencies
```

## 🛠️ CLI Reference

- `pnpm dev`: Start local preview server (watch mode)
- `pnpm build`: Build all slides to HTML in `dist/`
- `pnpm build:slides`: Build only user slides
- `pnpm pdf`: Export all slides to PDF
- `pnpm pptx`: Export all slides to PowerPoint

## 🤝 Contributing

Contributions are welcome! Please look at the [issues](https://github.com/chinkan/ai-marp-template/issues) to find something to work on.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.
