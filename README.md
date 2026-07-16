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
    ├── logo + brand marks        logo-wordmark(.png/-dark), logo-icon(.png/-dark), texas(.png/-dark), favicon
    ├── site-*.jpg                The Gasmer site and derrick (sunrise, sunset, blue sky, lake reflection)
    ├── ww-*.jpg                  Willow Waterhole Greenway (credited: Riese, Edmondson, Bloodworth)
    ├── mf-*.jpg                  MusicFest (two images only: Perme from-stage, gazebo sunset)
    ├── levitt-*.jpg              Levitt network venue cards (from Foundation composites)
    └── rendering-houston-wide.jpg  Early concept rendering (always captioned as concept)
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

## Support page structure

The Support page (support.html) runs two distinct, clearly labeled asks, matching standard nonprofit practice (Annual Fund vs. Capital Campaign, as seen at comparable orgs including Levitt San Jose and Valley Forge Park Alliance):

- **The Campaign** — the capital vision ask ("A New Kind of Energy for Houston"). No dollar figures, consistent with quiet-phase discipline.
- **Annual Fund** — ("Keep the Music Playing") supports MusicFest and yearly programming. Deliberately avoids naming a season, month, or event format, since neither is settled yet.

Both buttons currently point to the same Square link. See Outstanding for the tracking limitation.

## Roles & responsibilities

The site is under active editorial direction. Any change touching layout, imagery, or copy voice runs through a single review lens: national Levitt imagery carries the vision, the derrick carries the place, MusicFest carries proof of community. Images are visually verified before shipping; anything that fails verification becomes a labeled placeholder, never ships as-is.

## Verified facts (confirmed against levitthouston.org, current as of this build)

- Board of Directors and Advisory Board Members: matches the live site exactly. No year in the heading, matching the original editorial instruction.
- Mailing address: Friends of Levitt Pavilion Houston, Inc., 5300 N. Braeswood Blvd, Suite 4-202, Houston, TX 77096.
- Site location: 5521 Gasmer Drive, Houston, TX 77035 (not yet open to the public).
- All seven established Levitt venue "Official site" links point to each venue's real homepage, verified individually, not guessed.
- Media coverage: only one article is currently cited (Community Impact, 2020) because it is the only one I could verify has a real, working URL. Do not add placeholder-sounding media cards for outlets that haven't been confirmed to have covered the project; an empty or single-card section is more credible than invented-looking coverage.

## Image doctrine

Few images, all top quality. National Levitt venue photography and Willow Waterhole scenics carry the vision; the derrick photos carry the place; MusicFest gets exactly two images site-wide (proof of community, not competing with the national experience). No over-saturated/HDR-treated photography. Every image is visually verified before it ships; anything not clean gets a labeled placeholder instead. Unused files are deleted from /images, never parked.

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

- **Donation link** — both "Support Levitt" (Campaign) and "Give to the Annual Fund" buttons on the Support page point to the same Square checkout link (square.link/u/yzNNS96a). This works today but does not distinguish Campaign gifts from Annual Fund gifts in Square's reporting. Parked for a future backlog: set up separate Square items/links (or a memo field) if tracking the two funds separately becomes important.
- **Email capture endpoint** — real inline forms are now on Contact, Updates, and MusicFest (styled, accessible, ready to submit). Each has a placeholder Formspree action URL marked TODO. Fastest fix: create a free form at formspree.io and swap in the real endpoint on all three pages. Better long-term: if the org has (or gets) a Mailchimp/Constant Contact account, swap these forms for that platform's embed code so signups land in the same list as other supporters.
- Designer-produced branded location illustration for the Contact page (placeholder in place)
- Signature photography collection: additional MusicFest and Willow Waterhole photography as it becomes available (current set is intentionally small and high-quality; see Image doctrine above)
- SVG logo files from the designer, if/when produced (current build uses the extracted PNGs and that's a fine permanent state, not a blocker)
- Additional verified media coverage for the Updates page (currently one confirmed article; add more only when a real, checkable URL exists — see note below)
