# MOI Explorer (V2)

An interactive explorer of the STEM Innovation Academy Model of Instruction (MOI 2.0). Staff click a domain on the wheel to list its elements, then open any element for its summary, key takeaway, look-fors, rubric levels and pages from the MOI Teacher Reference Guide. A search box finds any element by keyword.

## What's in this folder

| File or folder | What it is |
| --- | --- |
| `index.html` | The whole explorer: layout, styles, element data and logo, all in one file. |
| `pages/` | The Teacher Reference Guide pages as images, `p6.webp` to `p95.webp`. Each element uses two pages, starting at 1.1 on page 6. |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are. |

## Publish with GitHub Pages

1. Create a new repository on GitHub, for example `moi-explorer`.
2. Upload everything in this folder to the repository, keeping the `pages` folder intact.
3. In the repository, go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to *Deploy from a branch*, choose the `main` branch and the `/ (root)` folder, then save.
5. After a minute or two the site is live at `https://<your-account>.github.io/moi-explorer/`.

To embed it on the school website, link to that address or place it in an iframe.

## Linking to one element

Every element has its own address. Add `#e` plus the element number with a dash to the site address, for example `.../moi-explorer/#e6-2` for 6.2 Engineering Design. Use these in emails or Teams posts.

## Updating it

- **Text, summaries or titles:** edit `index.html`. The element data is the `ELEMENTS` list near the top of the script.
- **Teams links:** near the top of the script in `index.html`, put your Teams folder link in `RESOURCES_DEFAULT` to use it for every element, or add element-specific links to `RESOURCES`, for example `"6.2": "https://..."`. Elements without a link show "Teams resources coming soon".
- **Look-fors, rubric text and key takeaways:** these are in the `GUIDE` list near the top of the script in `index.html`, keyed by element number (`k` takeaway, `t` teacher evidence, `s` student evidence, `r` the five rubric levels from Innovating to Not Using).
- **A new version of the reference guide:** replace the matching image in `pages/`, keeping the same file name (for example `p54.webp` for page 54).

The page loads the Big Shoulders Display and Nunito Sans fonts from Google Fonts. Everything else is in this folder.
