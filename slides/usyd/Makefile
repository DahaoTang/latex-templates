# =========================
# Project configuration
# =========================
MAIN        = slides
ENGINE      = xelatex
BIBENGINE   = biber
FLAGS       = -interaction=nonstopmode -file-line-error

# =========================
# Default target
# =========================
all: build clean

# =========================
# Build PDF
# =========================
build: $(MAIN).pdf

$(MAIN).pdf: $(MAIN).tex
	$(ENGINE) $(FLAGS) $(MAIN).tex
	$(BIBENGINE) $(MAIN)
	$(ENGINE) $(FLAGS) $(MAIN).tex
	$(ENGINE) $(FLAGS) $(MAIN).tex

# =========================
# Full Clean (Manual use only)
# =========================
clean:
	rm -f $(MAIN).{aux,bbl,bcf,blg,log,nav,out,run.xml,snm,toc,vrb}

distclean: clean
	rm -f $(MAIN).pdf

.PHONY: all build clean distclean