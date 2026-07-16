# Suture Lab — Emergency Medicine Medical Interest Club

> A single printable/browsable lesson-plan page for a high-school Emergency Medicine Medical Interest Club session: suturing, CPR, and tourniquet stations, an equipment shopping list, and cued-up videos — everything an instructor needs on one page.

![Status](https://img.shields.io/badge/status-not_deployed-lightgrey)
![Stack](https://img.shields.io/badge/HTML-static-black)
![Updated](https://img.shields.io/badge/last_updated-2026--07--16-blue)

**Live site:** not deployed yet — see To-do · **Site Editor:** not installed yet — add via the [Site Editor Kit](https://github.com/krs1jack/site-editor-kit) · **Last updated:** 2026-07-16 <!-- readme-last-updated -->

---

## Preview

screenshot pending — not yet deployed

<details>
<summary><strong>Tech stack</strong> — what it's built with, in plain English</summary>

| Technology | Version | What it does here (plain English) |
|---|---|---|
| HTML + inline CSS | — | This is one plain HTML file (`index.html`) with its styling built in — no framework, no build step, no server. Open it in any browser and it works. |

That's the whole stack. There's no JavaScript, no dependencies to install, and nothing to build.

</details>

<details>
<summary><strong>Related apps</strong> — other projects in this portfolio</summary>

- [Site Editor Kit](https://github.com/krs1jack/site-editor-kit) — the house no-code editor other sites use at `/admin`; not installed here (this page is simple enough to edit directly, see How to use below).
- Part of the wider MyHealthyCircle family of small, purpose-built pages.

</details>

<details>
<summary><strong>How to use</strong> — quick start for everyone, then technical setup</summary>

### For everyone (no coding needed)

This page is **not deployed to a live web address yet** (see To-do — the plan is to deploy it to Vercel or GitHub Pages). Until then:

1. Download or open `index.html` directly in any web browser (double-click it, or drag it into a browser window) to view the full lesson plan.
2. It covers: the session schedule, the two hands-on stations (Suturing; CPR & Trauma), the equipment/supplies list with Amazon links, videos to cue up beforehand, a resource-hub link section, and a quick instructor self-introduction prompt.
3. Print it or share the file with co-instructors before the session.

### Changing the session details (dates, room, schedule)

The date, room, and schedule are **hardcoded directly in `index.html`** — there's no settings file. To update them for a new session, open `index.html` in a text editor and change:

- **Room / location** — line 174: `📍 Hillside High School — Ms. Hood's Classroom, Room 210`
- **Time range** — line 175: `🕓 3:45 PM – 5:00 PM`
- **Date** — line 176: `📅 Tuesday, May 19`
- **Detailed schedule** — lines 182–190 (the `schedule-grid` block: arrival, intro, station rotations, wrap-up, food, end time)
- **Footer date/room line** — line 329: `Medical Interest Club · Suture Lab · May 19, 2026 · Hillside High School · Room 210`

### Technical setup (for developers)

```bash
git clone https://github.com/krs1jack/-suture-lab.git
cd -suture-lab
open index.html   # or just double-click it — no build step, no server needed
```

</details>

<details>
<summary><strong>Known issues</strong> — what doesn't work right today</summary>

- **Three resource links go nowhere:** the "Instructor Guide," "Student Worksheet," and "Full Resource Hub" links (lines 294–296) all point to `#` — they don't open anything yet.
- **Event details are hardcoded to one past session:** every date/room/schedule reference on the page (lines 174–176, 182–190, 329) is fixed to the "Tuesday, May 19" session at Hillside High School, Room 210. There's no way to reuse the page for a new session without manually editing the HTML (see How to use above).
- **Hotlinked Amazon and YouTube images:** the four equipment photos (lines 219, 227, 235, 243) load directly from `m.media-amazon.com`, and the three video thumbnails (lines 256, 267, 278) load directly from `img.youtube.com`. These aren't hosted in this repo, so they can break or change without notice, and every page view pings Amazon/YouTube's servers.
- **Not deployed:** there is no hosting configuration in this repo yet, so the page currently only works by opening the file locally.

</details>

<details>
<summary><strong>To-do — fixing & deploying</strong></summary>

- [ ] Deploy to Vercel or GitHub Pages so the page has a shareable live URL.
- [ ] Fill in real links for the three resource-hub buttons (lines 294–296), or remove them until they exist.
- [ ] Either generalize the schedule/date/room fields (e.g. pull them into a small config block at the top of the file) or clearly relabel the page as a specific past session's archive.
- [ ] Download and self-host the four equipment images and three video thumbnails instead of hotlinking them from Amazon/YouTube.

</details>

<details>
<summary><strong>Future improvements</strong> — ideas, not commitments</summary>

- Pull the date/room/schedule/equipment list into a small JSON config block (like other house apps) so future sessions can be updated without editing HTML/CSS.
- Add a print-specific stylesheet so the page formats cleanly when printed for in-person use.
- Add a simple no-code Site Editor so future club officers can update session details themselves.

</details>

<details>
<summary><strong>Version history</strong> — newest first</summary>

| Date | Version / change | What changed, in plain English |
|---|---|---|
| 2026-07-16 | README overhaul | This README: house-standard format, honest known-issues list, exact line references for editing session details. No page content touched. |
| 2026-05-19 | Update session schedule times | Session schedule times in `index.html` were updated. |
| 2026-05-19 | Rename to `index.html` | File renamed from `suture_lab_lesson_plan.html` to `index.html` so it can serve as a site's homepage. |
| 2026-05-19 | Initial upload | Initial lesson-plan page added. |

<!-- The readme-freshness workflow flags pushes that change code but add no row here. -->

</details>

<details>
<summary><strong>Security check</strong> — verified list + open issues</summary>

**Checks performed on 2026-07-16:** <!-- security-check-date -->

| Check | Result |
|---|---|
| Secret scan (API keys, tokens, private keys in code) | ✅ None found. |
| `.env` files kept out of git | ✅ None tracked (this is a static page with no environment config at all). |
| `npm audit` dependency vulnerabilities | ✅ Skipped — no `package.json`, no dependencies of any kind. |
| Outbound resources reviewed | ⚠️ The page hotlinks images from `m.media-amazon.com` and `img.youtube.com` (see Known issues). Not a secret-leak risk, but it does mean every page view contacts Amazon and Google's servers and depends on those images staying at those URLs. |

**Open security issues:**

- None involving secrets or credentials. The hotlinked third-party images above are a reliability/privacy note, not a security vulnerability, and are tracked in Known issues / To-do.

</details>

---

<sub>This README follows the house standard (see `TEMPLATE-README.md`). Structure is identical across all repositories: Preview → Tech stack → Related apps → How to use → Known issues → To-do → Future improvements → Version history → Security check.</sub>
