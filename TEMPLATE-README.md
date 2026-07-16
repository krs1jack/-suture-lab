<!--
  ══════════════════════════════════════════════════════════════════
  UNIVERSAL README TEMPLATE — Kim's standard for every repository
  ══════════════════════════════════════════════════════════════════
  STANDING RULE: Every new project starts from this template and
  includes the README auto-update workflow
  (.github/workflows/readme-freshness.yml). Copy this file into the
  new repo as TEMPLATE-README.md, fill in a copy as README.md, and
  add the workflow before the first release.

  HOW TO FILL IT IN
  - Replace every {{PLACEHOLDER}}. Delete any guidance comment like
    this one when done. No placeholder may survive into README.md.
  - Keep the section names and order EXACTLY as they are here — that
    is what makes every repo instantly familiar.
  - Sections 3–10 stay inside <details> blocks (collapsible) so the
    page opens short and calm.
  - Screenshots must show the app ACTUALLY RUNNING (live URL or local
    dev server), saved in docs/screenshots/ inside the repo.
  - The Security check section may only list checks that were REALLY
    performed, with the date they were run. Never rubber-stamp.
  - Write everything twice-friendly: technical facts, explained in
    plain English for non-coders.
-->

# {{APP NAME}}

> {{One plain-English sentence: what this app does and for whom.}}

![Status]({{shields.io badge, e.g. https://img.shields.io/badge/status-live-brightgreen}})
![Stack]({{shields.io badge for the main framework}})
![Updated](https://img.shields.io/badge/last_updated-{{YYYY--MM--DD}}-blue)

**Live site:** {{URL or "not deployed yet"}} · **Site Editor:** {{[/admin]({{live URL}}/admin) — edit this site's words, colors, and features with no code, or "not installed yet — add via the [Site Editor Kit](https://github.com/krs1jack/site-editor-kit)"}} · **Last updated:** {{YYYY-MM-DD}} <!-- readme-last-updated -->

---

## Preview

<!-- Live screenshots of the app actually running. 2–3 images, captured fresh. -->

| {{Page name}} | {{Page name}} |
|---|---|
| ![{{alt}}](docs/screenshots/{{file}}.png) | ![{{alt}}](docs/screenshots/{{file}}.png) |

<details>
<summary><strong>Tech stack</strong> — what it's built with, in plain English</summary>

| Technology | Version | What it does here (plain English) |
|---|---|---|
| {{Next.js}} | {{16.x}} | {{The framework that builds and serves the pages.}} |
| {{…}} | {{…}} | {{…}} |

</details>

<details>
<summary><strong>Related apps</strong> — other projects in this portfolio</summary>

- [Site Editor Kit](https://github.com/krs1jack/site-editor-kit) — the house no-code editor every site should carry at `/admin`; note here whether it's installed.
- [{{App}}]({{repo or live URL}}) — {{how it relates}}
- {{…}}

</details>

<details>
<summary><strong>How to use</strong> — quick start for everyone, then technical setup</summary>

### For everyone (no coding needed)

{{Numbered steps a non-coder can follow: open this URL, click this, etc.}}

### Technical setup (for developers)

```bash
{{git clone …
npm install
npm run dev}}
```

{{Environment variables table if any: name, required?, what it's for.}}

</details>

<details>
<summary><strong>Known issues</strong> — what doesn't work right today</summary>

- {{Issue, stated honestly, with where it shows up.}}

</details>

<details>
<summary><strong>To-do — fixing & deploying</strong></summary>

- [ ] {{Concrete next action needed to fix or ship.}}

</details>

<details>
<summary><strong>Future improvements</strong> — ideas, not commitments</summary>

- {{Improvement idea and why it would help.}}

</details>

<details>
<summary><strong>Version history</strong> — newest first</summary>

| Date | Version / change | What changed, in plain English |
|---|---|---|
| {{YYYY-MM-DD}} | {{v1.1 / "README overhaul"}} | {{…}} |

<!-- The readme-freshness workflow flags pushes that change code but add no row here. -->

</details>

<details>
<summary><strong>Security check</strong> — verified list + open issues</summary>

**Checks performed on {{YYYY-MM-DD}}:** <!-- security-check-date -->

| Check | Result |
|---|---|
| Secret scan (API keys, tokens, private keys in code) | {{✅ none found / ❌ details}} |
| `.env` files kept out of git | {{✅ / ❌}} |
| `npm audit` dependency vulnerabilities | {{✅ 0 found / ❌ N found — list}} |
| {{Any app-specific check actually run}} | {{result}} |

**Open security issues:**

- {{Honest list, or "None known as of the date above."}}

</details>

---

<sub>This README follows the house standard (see `TEMPLATE-README.md`). Structure is identical across all repositories: Preview → Tech stack → Related apps → How to use → Known issues → To-do → Future improvements → Version history → Security check.</sub>
