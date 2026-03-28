# Mphasis AI & Applied Tech Lab — Website

Website for the Mphasis AI & Applied Tech Lab at Ashoka University.

---

## Running locally

```bash
cd mphasis-lab-website
python3 -m http.server 8080
```

Then open [http://localhost:8080](http://localhost:8080).

---

## Folder structure

```
├── index.html               # Homepage
├── pages/
│   ├── about.html
│   ├── contact.html
│   ├── impact.html
│   ├── makerspace.html
│   ├── news.html
│   ├── people.html
│   ├── pillar.html          # Dynamic pillar detail page
│   ├── project.html         # Dynamic project detail page
│   ├── publications.html
│   └── research.html
├── src/
│   ├── assets/images/       # Logos, people photos, partner logos
│   ├── css/
│   │   ├── variables.css    # ← Edit colours, fonts, spacing here
│   │   ├── base.css
│   │   ├── components.css
│   │   └── ...
│   ├── data/
│   │   ├── people.js        # ← Add/edit team members here
│   │   ├── pillars.js       # ← Add/edit research pillars here
│   │   ├── projects.js      # ← Add/edit projects here
│   │   └── publications.js  # ← Add/edit publications here
│   └── js/
│       ├── main.js
│       └── gsap-animations.js
```

---

## How to edit content

### Adding a team member
Open `src/data/people.js` and add an entry to the array:

```js
{
  name: "First Last",
  role: "PhD Student",
  pillar: "ai",               // ai | bharatsim | chart | cyber | makerspace
  bio: "Short bio here.",
  image: "src/assets/images/people/first-last.jpg",
  links: {
    email: "email@ashoka.edu.in",
    website: "https://...",   // optional
    scholar: "https://...",   // optional
  }
}
```

### Adding a project
Open `src/data/projects.js`:

```js
{
  id: "unique-slug",
  title: "Project Title",
  pillar: "ai",
  status: "active",           // active | completed
  summary: "One-line summary.",
  description: "Full description.",
  team: ["Person Name"],
  tags: ["tag1", "tag2"],
}
```

### Adding a publication
Open `src/data/publications.js`:

```js
{
  title: "Paper Title",
  authors: ["Author One", "Author Two"],
  venue: "Conference / Journal Name",
  year: 2024,
  pillar: "ai",
  url: "https://...",         // link to paper
  abstract: "Abstract text.",
}
```

---

## Changing colours or fonts

All design tokens live in **`src/css/variables.css`**. Edit that file only — do not touch the other CSS files unless you know what you're doing.

Key tokens:

| Token | What it controls |
|-------|-----------------|
| `--color-primary` | Main brand colour (buttons, links, accents) |
| `--color-bg` | Page background |
| `--color-bg-dark` | Dark section background (hero, footer) |
| `--font-display` | Heading font |
| `--font-sans` | Body / UI font |
| `--pillar-ai` etc. | Per-pillar accent colours |

**Current fonts:** Barlow (headings) + Manrope (body). To change, update the Google Fonts `<link>` in `index.html` and all `pages/*.html`, then update `--font-display` and `--font-sans` in `variables.css`.

---

## Deploying

The site is plain HTML/CSS/JS — no build step needed. Push to `main` and GitHub Pages will serve it automatically from the repo root.

GitHub Pages URL: [https://ojastripathi1903.github.io/mphasis-ai-lab/](https://ojastripathi1903.github.io/mphasis-ai-lab/)
