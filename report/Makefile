SOURCES = $(wildcard *.tex)
OBJECTS = $(patsubst %.tex, %.pdf, $(SOURCES))

all: $(OBJECTS)

midterm.pdf: midterm.tex
	xelatex -halt-on-error $< -o $@
	xelatex -halt-on-error $< -o $@
	xelatex -halt-on-error $< -o $@
	open -a Preview $@

final.pdf: final.tex final/*.tex
	xelatex -halt-on-error $< -o $@
	xelatex -halt-on-error $< -o $@
	xelatex -halt-on-error $< -o $@
	open -a Preview $@

clean:
	rm -f *.log *.aux *.nav *.snm *.toc *.lof *.vrb *.out *.bbl *.blg *.synctex.gz *.bu
	find . -name *.aux -exec rm -f {} \;
