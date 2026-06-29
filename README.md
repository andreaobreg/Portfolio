# Andrea Obregon — Personal Website

My portfolio site. It's a single file: **`index.html`**. That's the whole website.

---

## How to edit it

The easiest way (no apps to install):

1. Go to my GitHub repo in the browser
2. Click on **`index.html`**
3. Click the **pencil icon ✏️** (top-right of the file)
4. Change the text
5. Click **Commit changes** at the bottom

Vercel automatically updates the live site within a few seconds. No re-uploading needed.

> Prefer editing on my computer instead? Open `index.html` in TextEdit or VS Code,
> make changes, save, and re-upload it to GitHub (Add file → Upload files).

---

## Where everything lives

The file is split into clearly labeled sections. Search for these comments to jump to the right spot:

| Comment in the file | What it controls |
|---|---|
| `<!-- HERO -->` | Name, tagline, intro line, buttons |
| `<!-- ABOUT -->` | The two "about me" paragraphs + the stats |
| `<!-- EXPERIENCE -->` | Jobs, internships, research |
| `<!-- SKILLS -->` | Skill cards (Research, Psychology, etc.) |
| `<!-- EDUCATION -->` | Northwestern + study abroad |
| `<!-- CLUBS -->` | Clubs & volunteering |
| `<!-- CONTACT -->` | Email + LinkedIn |

---

## Common edits — copy the pattern

**Change a paragraph / line of text:** just type over the words between `>` and `<`.

**Add a new club** — find `<!-- CLUBS -->`, copy one block and change the text:
```html
<div class="club-card">
  <div class="club-name">Name of the Club</div>
  <div class="club-role">My Role · 2026 – Present</div>
</div>
```

**Add a new job/experience** — find `<!-- EXPERIENCE -->`, copy one `exp-item` block:
```html
<div class="exp-item">
  <div class="exp-header">
    <div class="exp-role">My Title</div>
    <div class="exp-date">Month Year – Month Year</div>
  </div>
  <div class="exp-company">Organization — Location</div>
  <ul class="exp-bullets">
    <li>What I did.</li>
    <li>Another thing I did.</li>
  </ul>
</div>
```

**Add a skill tag** — inside any skill card, add:
```html
<span class="tag">My New Skill</span>
```

**Update my email or LinkedIn** — find `<!-- CONTACT -->` and change the
`mailto:` address or the LinkedIn URL.

---

## Things to leave alone

- The big `<style>` block at the very top controls all the colors and layout
  (the blue theme). Don't touch it unless I want to redesign.
- Keep the file named **`index.html`** — Vercel needs that name to serve the site.

---

## Tip

A safe way to experiment: change something, save/commit, and look at the live site.
If it breaks, GitHub keeps a history — I can always revert to the previous version
(repo → the file → "History" → pick an older version).
