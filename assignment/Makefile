FILE=main
CONTENT_DIR=content
REFERENCES_BIB=$(CONTENT_DIR)/references.bib
REFERENCES_AUX=$(FILE).aux
ALL_TEX=$(CONTENT_DIR)/*.tex

all: $(FILE).pdf

$(FILE).pdf: $(FILE).tex $(ALL_TEX) $(REFERENCES_BIB)
	pdflatex $(FILE).tex
	bibtex $(REFERENCES_AUX)

clean:
	@rm -rf *.aux *.bbl *.blg *dvi *.log *.out *.synctex.gz *.toc *.lot *.lof

.PHONY: clean all
