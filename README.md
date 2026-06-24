# Ous Bayaa — Portfolio

Single-file portfolio site. No build step — Tailwind loads from a CDN, so you just edit `index.html` and refresh the browser.

## Open in VS Code
1. Put `index.html` (and this README) in a folder.
2. In VS Code: **File → Open Folder…** → pick that folder.
3. Open `index.html`. To preview: right-click → **Open with Live Server** (install the "Live Server" extension), or just double-click the file to open it in your browser.

## What to edit (search the file for these markers)
- **`TODO`** — résumé links (nav, mobile menu, hero) and the contact-form handler note.
- **`EDIT ME`** — the `PROJECTS` array near the bottom `<script>`. Three real entries are filled in; three are placeholders for your side projects. Each project is an object:
  ```js
  {
    id: 'unique-id',
    cat: 'qa' | 'web' | 'insurance',   // controls which filter shows it
    catLabel: 'QA & Testing',
    type: 'Side project',
    title: 'Project name',
    blurb: 'One line shown on the card.',
    body: 'Longer text shown in the View Details modal.',
    tags: ['Python', 'Pytest'],
    status: 'LIVE',                      // small chip on the card
  }
  ```
- **Social URLs** — currently guessed (`linkedin.com/in/ousbayaa`, `github.com/ousbayaa`). Replace in the hero and footer.

## Colors & fonts
At the top of the `<style>` block, `:root` (light) and `.dark` (dark mode) hold every color as a CSS variable. Change one value, both the component and its dark variant update.

## Deploy (Cloudflare Pages)
Drag the folder into a new Pages project, or push to GitHub and connect the repo. The output directory is the folder itself (no build command needed).
