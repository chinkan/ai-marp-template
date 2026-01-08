---
marp: true
theme: developer
paginate: true
header: 'Marp Template Guide'
footer: 'AI-Powered Slide Generation'
---

# Marp Template
## AI-Powered Slide Generation

A template for creating beautiful presentations with Marp and AI assistance.

---

# Quick Start

## Generate a New Presentation

Simply type `@slide` followed by your topic and key points:

```text
@slide
Topic: Your Presentation Title
Points:
- First key point
- Second key point
- Third key point
```

The AI will create a new slide deck in `src/slides/`.

---

# Update Existing Slides

## Modify Your Presentation

Use `@slide-update` to modify an existing presentation:

```text
@slide-update
Add a slide about performance metrics after the introduction
```

The AI will read your current slide file and apply changes.

---

# Project Structure

```
src/
├── slides/     # Your presentations
├── demo/       # Theme examples
├── themes/     # Custom CSS themes
└── assets/     # Images, icons, videos
```

---

# Available Themes

| Theme | Best For |
|-------|----------|
| `default` | General purpose |
| `gaia` | Clean, minimal |
| `uncover` | Bold statements |
| `corporate` | Business presentations |
| `developer` | Code-heavy talks |
| `gradient` | Marketing, creative |

---

# Using Themes

Set the theme in your front-matter:

```yaml
---
marp: true
theme: corporate
paginate: true
---
```

Browse `src/demo/` to see theme examples.

---

# Slide Syntax Basics

## Separating Slides

Use `---` between slides:

```markdown
# Slide 1

Content here...

---

# Slide 2

More content...
```

---

# Background Images

## Full Background

```markdown
![bg](./assets/images/photo.jpg)

# Title Over Image
```

## Split Layout

```markdown
![bg right:40%](./assets/images/photo.jpg)

# Text on Left
- Point 1
- Point 2
```

---

# Per-Slide Customization

## Local Directives

```markdown
<!-- _class: invert -->
<!-- _backgroundColor: #1a1a2e -->

# Dark Slide

This slide has custom styling.
```

The underscore `_` means "this slide only".

---

# Scoped CSS

## Custom Styles for One Slide

```markdown
<style scoped>
section {
  background: linear-gradient(45deg, #12c2e9, #c471ed);
  color: white;
}
</style>

# Gradient Slide
```

---

# Code Highlighting

## Syntax Highlighting Built-in

```javascript
async function fetchData(url) {
  const response = await fetch(url);
  return response.json();
}
```

Always specify the language after triple backticks.

---

# CLI Commands

```bash
# Development server with hot reload
pnpm dev

# Build all slides to HTML
pnpm build

# Export to PDF
pnpm pdf

# Export to PowerPoint
pnpm pptx
```

---

# Tips for AI Generation

1. **Be specific** - Include topic, audience, and key points
2. **Mention theme** - "Use the developer theme"
3. **Specify length** - "Create a 10-slide presentation"
4. **Add context** - "This is for a tech conference"

---

# Example Prompt

```text
@slide
Topic: Introduction to Docker
Audience: Junior developers
Theme: developer
Points:
- What is containerization?
- Docker vs VMs
- Basic Docker commands
- Dockerfile basics
- Docker Compose intro
```

---

# Resources

- **Marp Documentation**: [marp.app](https://marp.app)
- **Marpit Framework**: [marpit.marp.app](https://marpit.marp.app)
- **Theme CSS Guide**: `src/demo/theme-showcase.md`

---

<!-- _class: invert -->

# Start Creating!

Run `pnpm dev` and open http://localhost:8080

Type `@slide` with your ideas to generate presentations.

**Happy presenting!**
