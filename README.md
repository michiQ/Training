# Selling the Strategy Collection

Internal sales enablement for Focus, Talent and Jira Product Discovery. Built from Atlassian's partner materials and Praecipio's Planning Flow and Strategy Stack visuals.

## Pages

| File | What it is |
|---|---|
| `index.html` | The training site: eight modules, about 45 minutes, with "hear it, say it" lines and quick checks |
| `practice.html` | Daily practice: five drills a day, browse by play, one-screen cheat sheet |
| `planning-flow.html` | Praecipio Planning Flow, full detail |
| `strategy-stack.html` | AI-Age Strategy Stack diagram |

All pages are self-contained HTML (images embedded, no build step). Fonts load from Google Fonts; everything else works offline. Progress and streaks are stored in the browser with `localStorage`, per person, per browser.

## Hosting

Any static host works. For GitHub Pages: Settings → Pages → deploy from the `main` branch root. The site is then at `https://<org>.github.io/<repo>/`.

## Editing content

All copy lives in the `<script>` block of each page:

- `index.html`: the `MODULES` array (one object per module: `body` HTML, `hs` hear-it/say-it pairs, `checks` quick-check questions)
- `practice.html`: `ROUTE` (hear it, route it), `RESPOND` (pick the reply), `PERSONA` (open the conversation), `TERM` (flashcards), and the cheat sheet in `renderSheet()`

Two Loom walkthroughs are embedded in modules 2 and 5 of the training site.

## Sources

Atlassian Partner Portal (login required): Strategy Collection and Jira Product Discovery pages, including the use cases, personas and ICP, positioning guide, pricing and packaging, Talent and Viewer quick references, the JPD Sales Guide and the Product Discovery Handbook.
