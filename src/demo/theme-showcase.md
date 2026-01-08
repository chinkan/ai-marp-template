---
marp: true
theme: default
paginate: true
header: 'Marp Themes Overview'
footer: 'Custom Theme Guide'
---

# Marp Custom Themes
## Theme Selection Guide

This project includes 5 custom themes for different use cases.

---

# Available Themes

| Theme | File | Best For |
|-------|------|----------|
| **corporate** | `theme-corporate.md` | Business, formal |
| **developer** | `theme-developer.md` | Tech talks, code |
| **gradient** | `theme-gradient.md` | Marketing, creative |
| **minimal** | `theme-minimal.md` | Academic, clean |
| **midnight** | `theme-midnight.md` | Executive, evening |

---

# Important: Theme Limitation

In Marp, the `theme` directive is **global only**.

You **cannot** change themes per-slide within a single presentation.

```yaml
---
marp: true
theme: corporate  # Applies to ALL slides
---
```

---

# Per-Slide Customization

While you can't switch themes, you CAN customize individual slides:

1. **`_class: invert`** - Dark/light variant
2. **`_backgroundColor`** - Custom background
3. **`<style scoped>`** - Scoped CSS rules

---

# Scoped Style Example

```markdown
<style scoped>
section {
  background: linear-gradient(to right, #fc5c7d, #6a82fb);
  color: white;
}
</style>

# This slide has custom styling
```

Use `<style scoped>` for one-off slide customizations.

---

# View Theme Demos

Open these files to see each theme in action:

- `src/demo/theme-corporate.md` - Professional blue theme
- `src/demo/theme-developer.md` - Dark mode for code
- `src/demo/theme-gradient.md` - Vibrant gradients
- `src/demo/theme-minimal.md` - Clean & simple
- `src/demo/theme-midnight.md` - Elegant dark mode

Run `pnpm dev` and navigate to each file.
