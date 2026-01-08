---
marp: true
theme: developer
paginate: true
header: 'Developer Theme Demo'
footer: 'Code-First Presentations'
---

# Developer Theme
## Dark Mode for Technical Presentations

Optimized for code readability and eye comfort

---

# Theme Features

- **Typography**: Fira Code / Consolas monospace
- **Colors**: VS Code-inspired dark palette
- **Background**: Dark gray (#1e1e1e)
- **Syntax**: High contrast for code blocks

> Ideal for tech talks, code reviews, and demos

---

# JavaScript Example

```javascript
async function fetchUserData(userId) {
  const response = await fetch(`/api/users/${userId}`);
  if (!response.ok) {
    throw new Error(`HTTP ${response.status}`);
  }
  return response.json();
}
```

---

# Python Example

```python
def fibonacci(n: int) -> list[int]:
    """Generate Fibonacci sequence up to n terms."""
    if n <= 0:
        return []
    sequence = [0, 1]
    while len(sequence) < n:
        sequence.append(sequence[-1] + sequence[-2])
    return sequence[:n]
```

---

# Shell Commands

```bash
# Build and deploy
npm run build
docker build -t myapp:latest .
docker push registry.example.com/myapp:latest
kubectl rollout restart deployment/myapp
```

---

# Architecture Overview

```
┌──────────────┐     ┌──────────────┐
│   Frontend   │────▶│   API Gateway │
└──────────────┘     └──────┬───────┘
                            │
              ┌─────────────┼─────────────┐
              ▼             ▼             ▼
        ┌─────────┐   ┌─────────┐   ┌─────────┐
        │ Service │   │ Service │   │ Service │
        │    A    │   │    B    │   │    C    │
        └─────────┘   └─────────┘   └─────────┘
```

---

# Questions?

Find me on GitHub: **@developer**
