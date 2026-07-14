# Levitt Pavilion Houston — Website

Public website for Friends of Levitt Pavilion Houston (FLPH), the Texas nonprofit building and programming Levitt Pavilion Houston beside Willow Waterhole Greenway in Southwest Houston.

**Live site:** https://jbroadfoot.github.io/levitthouston-site
(Future custom domain: levitthouston.org)

## What this is

A pure HTML/CSS static site. No framework, no build step, no dependencies beyond Google Fonts loaded at runtime. Anything you see in this repo is exactly what ships. Hosting is free via GitHub Pages.

## Structure

```
/
├── index.html        Homepage: hero, four pillars, campaign band, network proof, MusicFest, CTA
├── vision.html       The site, the plan, the derrick and Light the Star, front door + pipeline
├── network.html      The national Levitt network and Foundation partnership
├── musicfest.html    Our annual festival, proof of concept
├── partners.html     MOU partners and community coalition
├── support.html      Capital campaign, Light the Star giving opportunity, ways to give
├── about.html        Who we are, board, Willow Waterhole roots
├── news.html         Project Updates: timeline of milestones (nav label is "Updates")
├── contact.html      Lightweight contact page (linked from the footer, not main nav)
├── styles.css        Shared design system for every page
└── images/
    ├── logo-wordmark.png        Primary mark, light backgrounds (nav)
    ├── logo-wordmark-dark.png   Primary mark, dark backgrounds
    ├── logo-icon.png            Derrick icon, light backgrounds
    ├── logo-icon-dark.png       Derrick icon, dark backgrounds (homepage hero)
    ├── texas.png                Texas mark, light backgrounds
    ├── texas-dark.png           Texas mark, dark backgrounds (footer)
    └── favicon.png              Browser tab icon
```

PNG logos were extracted from the designer's PDF. When SVG files arrive from the designer, replace the PNGs (keeping the same filenames with .svg extensions and updating the `<img src>` paths) for crisper scaling.

## Design system

Defined entirely in `styles.css`.

- **Palette:** Charcoal `#292929`, Cream `#F8F4F3`, Orange `#FF6F32`, Blue `#43A1D5`
- **Color discipline:** Orange means action (Donate, campaign CTAs, eyebrow labels, the "Ahead" timeline marker). Blue means place and credibility (facts and stats, completed milestones, the current-page nav marker, wave dividers, water in the illustrations). Charcoal and cream carry the sophistication; orange and blue are accents, used sparingly.
- **Type:** Archivo (display, uppercase, echoes the wordmark) + Lora (body, narrative warmth), loaded from Google Fonts.
- **Components:** cards (`.card`, `.card-blue`), stats (`.stat`, `.stat-blue`), timeline, pullquote, wave divider (callback to the water in the logo), momentum bar, campaign band (the "A new kind of energy" moment).

## How to update

Every page is standalone HTML. To edit copy, open the file, find the text, change it, commit. The nav and footer are duplicated on every page, so a change to either must be made in all eight files.

**Editing in the GitHub web UI:** open the file, click the pencil icon, edit, commit to `main`.

**Adding images:** GitHub's drag-and-drop upload flattens folders. To place a file inside `/images`, use "Add file → Create new file" or the upload dialog and type `images/filename.png` in the name field; GitHub creates the folder path automatically.

## Deployment

GitHub Pages serves the `main` branch automatically. Any commit to `main` is live within a minute or two. There is nothing to build or configure.

## Content rules (important)

Site copy follows the Editorial Standards Guide (`EDITORIAL-STANDARDS.md` in this repo) and the internal Brand & Message Platform. The rules that most often come up when editing:

1. **No financial figures of any kind.** No grant amounts, operating support figures, campaign totals or targets, or lease values. The campaign is in a quiet phase; confidence comes from vision, not numbers.
2. **No agreement mechanics.** No MOU, lease terms, governance structures, maintenance agreements, or committee language.
3. **Safe facts only:** 40 to 50 free concerts annually; approximately 8 acres; the 291-acre greenway; ~350,000 residents within five miles; network stats (1974, 100+, 1,000+, 1M+). No capacity figures or dates until confirmed.
4. **Status language:** planning continues; the project continues to advance; future milestones are anticipated, not committed.
5. **The star is proposed.** Always "a proposed crowning element of the restored derrick, subject to site design."
6. **No park name, no acronyms** (TIRZ, MOU, FLPH, LCCA) in public copy. "Southwest Houston Redevelopment Authority" in full.
7. **Taglines:** "A new kind of energy" is the campaign voice. "Free live music under the stars" is the experiential line. "Building community through music" is for formal, Foundation-facing use.

## Outstanding

- Active donation platform URL (Give Online button points to the legacy site; TODO comment marks it in support.html)
- Mailing address for Contact page and footer (marked TODO; footer shows the future pavilion location, 5521 Gasmer Drive)
- Exact headlines, dates, and article URLs for the three In the Media cards (Updates page; links currently go to publication homepages)
- Official per-venue site URLs on the Network page (currently levitt.org with TODOs)
- Designer-produced branded location illustration for the Contact page (placeholder in place)
- Embedded email sign-up form (mailto links are weak capture; consider Mailchimp or similar)
- Signature photography collection: aerials, the derrick, Willow Waterhole, MusicFest crowds, families, authentic Levitt venue photos
- SVG logo files from the designer
