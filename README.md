# weave-dithering
an online generator that converts user uploaded images to a combination of stitching, punches, or binaries. inspired by charles babbage, jacquard loom, and weaving notations

## Point Paper Loom

A cover generator for my portfolio. The page is weaving point paper. A floral frame is drawn on it cell by cell, and the cells pass through three states in order: stitched, punched, then read as binary. The share of each state, where the binary starts, the marks, the pen weights, the colours and the type are all adjustable. A reference image can be dithered into the same states.

It is one self-contained HTML file with no build step. Open `index.html` in a browser, or use it live at https://mentaldogfood.github.io/weave-dithering/ once GitHub Pages is on.

## What it does

- **Paper:** Letter by default, with other sizes, orientation, margins and grid resolution.
- **Pattern:** two generated frames (sampler and minimal), an uploaded image, or both. Images are dithered with Floyd–Steinberg, Atkinson, Bayer 4×4 or a threshold.
- **Marks:** blind emboss, cross stitch (flat, floss or wool), pen X and slash, punched dots and ovals, and binary digits in cells or on grid intersections.
- **Yarn:** wool keeps the cross-stitch pattern but draws each leg as two plies twisted into slanted lumps, with combed surface fibres. Halo adds loose fibre around the yarn. Strays leave loose threads trailing from the stitches, as a random walk of 3–8 steps smoothed into one twisted strand.
- **Line:** grid as lines, crosses, dots, or lines and dots. Each has its own weight and colour, with hand wobble and uneven ink.
- **Type:** the title block follows my InDesign styles: Adobe Garamond Pro for display, and Neue Haas Grotesk for the date and captions.
- **Export:** 300 dpi PNG, SVG sized in inches, and a TXT stitch chart.

Palettes, pen sets and profiles save to this browser's local storage. They don't sync between browsers or devices.

## Fonts

Adobe Garamond Pro and Neue Haas Grotesk are Adobe Fonts and can't be served from a public page. The page falls back to EB Garamond and Arimo from Google Fonts. For print, set final type in InDesign.

Anna Geng, 2026
