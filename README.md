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

## How to use

_Notes: the following building process triggered by saving the `.tex` file can only be successful when it builds successfully._

To build with a Makefile:

1. In the terminal, just stay at the root directory (or actually no matter where you are).
2. Go to `./cv`, `./poster` or `./slides` folder depending on your need.
3. Modify the `xxx.tex` file.
4. Save it -- it will automatically be built. Only the `slides.pdf` will be kept after the build -- all the other files will be removed.
