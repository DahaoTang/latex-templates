# Dahao's Latex Template

This repo serves as the template for LaTeX-based projects, e.g., slides, posters, etc.

The current templates include:

```
.
├── cv				# a standard latex cv
├── poster
│   └── usyd        # a USYD-inspired colour theme template for poster
├── slides
│   ├── casual      # a deep-blue theme
│   └── usyd        # a USYD-inspired colour theme template for slides
```

To make the template simple and easy-to-use, after careful consideration, the current template uses **_only one centralised_** `.sty` file which contains the font, colour, and structural design that tend to be kept in different files by beamer convention.

## How to use

_Notes: the following building process triggered by saving the `.tex` file can only be successful when it builds successfully._

To build with a Makefile:

1. Copy and paste (i) `assets/`, (ii) `fonts/`, (iii) `beamerthemeusyd.sty` (or `beamerthemeusydposter.sty`), (iv) `slides.tex` (or `poster.tex`) and (v) `Makefile` in the _same target folder_. These 5 folders/files are the only sources required to build a poster or slides.
2. Modify the `slides.tex` (or `poster.tex`) file with your content.
3. _(Optional) You may change the name of the `.tex` file. Make sure in the `Makefile`, the value assigned to `MAIN` aligns with the name of the `.tex` file._
4. Save it -- it will automatically be built. Only the `.pdf` will be kept after the build -- all the aux files will be removed.
