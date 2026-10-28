# Project Arche

The website for Project Arche, a four-month discovery programme for children aged 5–9.

**Website:** https://project-arche.oluwabukola-1974.chatgpt.site

## Pages

- **Home:** programme introduction and interactive lab previews.
- **About:** cohort overview, mission and vision.
- **How it works:** four-month lab sequence, learning rhythm and FAQs.
- **Curriculum:** programme outline and a space for future learning materials.

## Run locally

This is a static website. No package installation or build step is required.

```sh
git clone https://github.com/Big-debs/project-arche.git
cd project-arche
python3 -m http.server 8000 --directory dist
```

Open http://localhost:8000.

## Edit the website

- Page content: `dist/index.html`, `dist/about/index.html`, `dist/how-it-works/index.html`, `dist/curriculum/index.html`.
- Styles and responsive layouts: `dist/styles.css`.
- Mobile navigation and lab interactions: `dist/script.js`.
- Images and icons: `dist/assets/`.

The home page currently reserves a space for the owner's replacement image. Detailed curriculum materials are still to be added. Mission and vision copy remain available for editorial review.

## Programme structure

Four four-week labs in sequence: Design & Engineering, Futures, Culture, and Media. Ages 5–9, maximum 12 children, three days per week, five learning hours per day. The daily one-hour Village block, speedcube, abacus and spatial reasoning continue throughout the cohort. Individual work and a collective build culminate in the Builders Assembly.

## Validation

```sh
node --check dist/script.js
```

All four pages were checked in Chrome at viewport widths of 320, 375, 390, 600, 768, 820, 1024 and 1440 CSS pixels without horizontal overflow. Mobile menu opening, Escape dismissal, short-screen access and the lab selector were also checked.

## Hosting

Serve `dist/` as the static website directory. The existing ChatGPT Sites deployment is described by `.openai/hosting.json`. GitHub is the source repository; a push alone does not publish a new Site version.
