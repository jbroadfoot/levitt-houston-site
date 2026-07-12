# Levitt Pavilion Houston Site — Build List

Last updated: this session. Keep this file in the repo root and update it as we go.

## Done this session

- [x] Extracted real logo artwork from designer's PDF (not a recreation): wordmark light/dark, icon light/dark, Texas mark light/dark
- [x] Replaced nav and hero graphics with actual logo files
- [x] Removed hero animation, static icon now
- [x] Rebalanced orange: quieted the momentum bar and homepage closing CTA, orange now reserved for donate/action moments
- [x] Added blue accent system: place and partnership facts use blue, campaign dollar figures stay orange
- [x] Added wave divider (blue, quiet) at two place/credibility transitions: Vision and Partners pages
- [x] Blue top-border on the three Levitt network venue cards
- [x] Confirmed proper folder structure: images live in an `images/` subfolder, code points to `images/logo-wordmark.png` etc. (the right long-term structure, not flat files at repo root)

## What went wrong last time, and the fix

Dragging the 6 PNG files directly onto GitHub's upload screen flattened them into the repo root instead of preserving an `images/` folder. GitHub's uploader only preserves folder structure if you drag the **folder itself**, not its contents.

**Fix: use `images-folder.zip`.**
1. On the repo page, click "Add file" > "Upload files"
2. Drag `images-folder.zip` onto the upload area
3. GitHub will show a checkbox: "Automatically expand compressed files" (or similar wording depending on version) — check it if offered, this unzips into a real `images/` folder
4. If GitHub does not offer to expand the zip automatically, unzip it on your own computer first (double-click the zip in Downloads, it creates an `images` folder), then drag that unzipped `images` folder itself onto the GitHub upload screen
5. Also drag in the updated HTML files below (they now point to `images/filename.png`)
6. Commit

## Outstanding / needs your input

- [ ] Confirm `images/` folder shows correctly nested in the GitHub file list (not flat at root)
- [ ] Add a `README.md` to the repo: what the site is, folder structure, how to update content, how to redeploy
- [ ] Board member names and one-line bios for About page (currently placeholder cards)
- [ ] MusicFest 2026 date, once set, so I can add Event schema for Google
- [ ] Real photos: SteelStacks and Denver lawn shots are still striped placeholders. Best move is asking Sharon's team for approved network photos, plus any MusicFest 2025 photos you have
- [ ] Density pass: Vision, Network, and Partners pages still run a bit heavy, agreed to trim once content is stable
- [ ] SVG logo files from your designer, when available, to replace the extracted PNGs (gains transparency, cleaner scaling)
- [ ] Brand guideline one-pager, pull from what's built once site is settled, reconcile against designer's own brand doc when it lands

## Parked ideas, no action yet

- Texas mark with Houston music note: added to About page, "Our Roots" section. Could also work as a small footer mark or a favicon.
- Blue vs orange ratio is provisional. When your designer's brand document arrives, reconcile against their intended usage ratio.
