# BioRouter Landing Site

Static landing site for **BioRouter v1.20.0** — a local-first AI routing layer for clinical research developed at the [Baranzini Lab](https://baranzinilab.ucsf.edu/), UCSF.

**Live site:** <https://baranzinilab.github.io/biorouter-landing/>

---

## Pages

| File | Tab | Description |
| ---- | --- | ----------- |
| `index.html` | — | Redirects to `intro.html` |
| `intro.html` | Introduction | Hero section, feature highlights, supported AI providers |
| `download.html` | Download | OS-aware download card (auto-detects macOS arm64/x64, Windows, Linux), platform table, setup instructions |
| `docs.html` | Documentation | Sidebar-navigated documentation covering installation, configuration, recipes, federation, and CLI reference |
| `baam.html` | BAAM Marketplace | BioRouter AI Agent Marketplace — agent cards, install instructions, and community recipes |
| `about.html` | About | News & announcements, related links, acknowledgments, developer info |

### Shared assets

- `shared.css` — design tokens, navbar, buttons, tables, and all shared component styles
- `icon.png` — BioRouter app icon
- `assets/ehr-diabetes-recipe.yaml` — downloadable example recipe (EHR Diabetes Demographics Dashboard)
- `assets/landing-site-content.md` — content requirements tracker

---

## Design System

- **Theme:** Light warm background (`#ffffff` / `#fcf8ed` cream / `#f8f2df` beige)
- **Accent:** Coral/orange `#cf6d47` — matches the BioRouter desktop app
- **Text:** Warm dark `#2a2520`, muted `#7a736c`
- **Fonts:** [Inter](https://fonts.google.com/specimen/Inter) (body) + [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono) (code) via Google Fonts
- **Responsive:** Mobile hamburger menu at ≤768px

---

## Hosting

The site is hosted via **GitHub Pages** from the `main` branch root.

- **Repo:** <https://github.com/BaranziniLab/biorouter-landing>
- **Live URL:** <https://baranzinilab.github.io/biorouter-landing/>
- **Branch:** `main` → served from `/` (repo root)
- **Build:** None required — fully static HTML/CSS/JS, no build step

### Deploying updates

```bash
git add .
git commit -m "your message"
git push origin main
```

Changes go live automatically within ~1 minute after push. GitHub Pages rebuilds on every push to `main`.

### Local preview

Open any HTML file directly in a browser, or use a local server to avoid cross-origin issues with relative paths:

```bash
# Python
python3 -m http.server 8080

# Node (npx)
npx serve .
```

Then visit `http://localhost:8080`.

---

## Acknowledgements

### The Baranzini Lab — [baranzinilab.ucsf.edu](https://baranzinilab.ucsf.edu/)

- Gianmarco Bellucci
- Sergio Baranzini

### Bakar Computational Health Sciences Institute (BCHSI) — [bakarinstitute.ucsf.edu](https://bakarinstitute.ucsf.edu/)

- Sharat Israni
- Marina Sirota

### UCSF Academic Research Services (ARS) — [ars.ucsf.edu](https://ars.ucsf.edu/)

- William Santo
- Evan Philps
- Rick Larson
- Oksana Gologorskaya

### Open Source Inspirations

- **[Goose](https://block.github.io/goose/)** — CLI/Desktop agent for full developer workflows (Block) — BioRouter's primary upstream foundation
- **[Aider](https://aider.chat/)** — Open-source, Git-native CLI AI coding agent
- **[Cline](https://github.com/cline/cline)** — Open-source interactive CLI coding agent
- **[OpenCode](https://opencode.ai/)** — Open-source coding agent with multi-session and multi-provider support
- **[ForgeCode](https://forgecode.dev/)** — Terminal AI coding assistant for task planning and code generation

---

## Related

- **BioRouter app repo:** <https://github.com/BaranziniLab/BioRouter>
- **Baranzini Lab:** <https://baranzinilab.ucsf.edu/>
- **UCSF Versa:** <https://ai.ucsf.edu/platforms-tools-and-resources/ucsf-versa>
