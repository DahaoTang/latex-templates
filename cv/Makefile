MAIN=cv
OUT=out
LATEXMK=latexmk
LATEXMKFLAGS=-xelatex -synctex=1 -interaction=nonstopmode -file-line-error -outdir=$(OUT)

.PHONY: all clean watch

all:
	$(LATEXMK) $(LATEXMKFLAGS) $(MAIN).tex

clean:
	$(LATEXMK) -C -outdir=$(OUT)

watch:
	$(LATEXMK) $(LATEXMKFLAGS) -pvc $(MAIN).tex
