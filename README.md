# Joshua Lee · 이용준 — Interactive Résumé

**Live site:** https://jankykohh-boop.github.io/Portfolio/
**Résumé (PDF):** [resume.pdf](resume.pdf)

Network engineer, creator of Zennix, and a security-first builder. This repo is my résumé as an interactive site, built to read like the tools I work in every day: file paths, tickets, a terminal and a change queue.

## What's on the page

| Section | What you'll find |
|---|---|
| `~/README.md` | Cover with a live terminal (`whoami`), my Korean name and 도장 seal |
| `~/about` | Summary, impact numbers and skills |
| `~/zennix` | The legal-AI product I'm building: what I own, and the security checklist every change goes through |
| `~/experience` | A `traceroute` of my career, and my work filed as ServiceNow-style tickets you can filter by company |
| `~/certs` | B.S. in Cybersecurity, CompTIA and ISC2 |
| `~/contact` | Email, LinkedIn and the PDF résumé |

## Things to try

- **Folder-tab dock** at the bottom: click a tab to jump to that section.
- **Keyboard:** `1`–`6` jump between sections; `Ctrl+K`, `?` or `/` open a command palette (jump, copy email, toggle theme, open résumé).
- **Light / dark** toggle in the status bar.
- **Move your mouse** over the background: the network reaches toward your cursor over a Korean window-lattice (창살) pattern.

## How it's built

- **One HTML file**, no framework, no build step and no dependencies. Fonts come from Google Fonts (Archivo, JetBrains Mono, Syncopate, Noto Sans KR).
- **Accessible by default:** keyboard navigation, screen-reader labels, and all animation turns off when the visitor's device asks for reduced motion.
- **Résumé from the same source of truth:** `resume.html` is a print-styled page that exports to a one-page, ATS-friendly `resume.pdf`.
## Design credit

The folder-tab layout started from a [21st.dev portfolio template](https://21stdev-my-components-one.vercel.app/#folder-tab-portfolio-template). I made it my own: a black, navy, red and gold palette, my Korean name, 도장 seal and lattice background, and a "tech, not design" voice with file paths, tickets, a terminal and a status bar in place of a design portfolio's look.

## Files

```
index.html    the interactive résumé
resume.html   print layout for the PDF
resume.pdf    one-page résumé (generated from resume.html)
```

## Run it locally

Open `index.html` in any modern browser. That's it.

To regenerate the PDF after editing `resume.html` (Windows, Chrome):

```bash
"C:/Program Files/Google/Chrome/Application/chrome.exe" --headless=new --no-pdf-header-footer --virtual-time-budget=8000 --print-to-pdf="resume.pdf" "resume.html"
```

The résumé must stay on one page; check the PDF after any content change.

## Contact

janktester@gmail.com · [LinkedIn](https://www.linkedin.com/in/joshua-lee-b182b2149)

© Joshua Lee. Content and résumé are mine; please don't reuse them as your own.
