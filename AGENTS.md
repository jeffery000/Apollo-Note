# AGENTS.md

## Cursor Cloud specific instructions

This is a **documentation-only repository** (Apollo-Note) containing Chinese-language study notes about Baidu's Apollo 3.0 autonomous driving platform. There is **no executable source code, no build system, no package manager, and no services** in this repository.

### Repository structure

- `README.md` — Table of contents (Chinese) linking to all documentation
- `docs/` — Detailed module analysis in Markdown
  - `docs/perception/` — Perception module notes (LiDAR, Radar, Camera, Traffic Lights)
  - `docs/prediction/` — Prediction module notes
  - `docs/planning/` — Planning module notes
- `images/` — Architectural diagrams (PNG)

### Development workflow

Since this is a pure documentation repository:

- **Lint**: `markdownlint "**/*.md"` (requires `markdownlint-cli` installed globally via npm)
- **Preview/Serve**: `python3 -m http.server 8080` from the workspace root to browse docs locally
- **No tests**: There are no automated tests to run
- **No build**: There is no build step

### Important notes

- All documentation is in Chinese (Simplified)
- The docs contain inline HTML anchors (`<a>` tags) for navigation, which triggers markdownlint MD033 warnings — this is intentional
- Images are referenced with relative paths from the docs
- There are no dependencies to install beyond the optional linting tool
