# =========================
# Project configuration
# =========================
MAIN    = slides
ENGINE  = xelatex
FLAGS   = -interaction=nonstopmode -file-line-error

# =========================
# Default target: build + clean
# =========================
all: build clean-aux

# =========================
# Build PDF (2-pass for beamer)
# =========================
build: $(MAIN).pdf

$(MAIN).pdf: $(MAIN).tex
	$(ENGINE) $(FLAGS) $(MAIN).tex
	$(ENGINE) $(FLAGS) $(MAIN).tex

# =========================
# Clean auxiliary files only
# =========================
clean-aux:
	rm -f $(MAIN).{aux,bcf,log,nav,out,snm,toc,vrb,fls,fdb_latexmk,synctex.gz,run.xml}

# =========================
# Full clean (manual use)
# =========================
clean: clean-aux

distclean: clean
	rm -f $(MAIN).pdf

.PHONY: all build clean clean-aux distclean
