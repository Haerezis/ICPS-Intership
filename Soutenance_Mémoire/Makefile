NAME = Soutenance_Mémoire
SRC = $(NAME).tex
PDF = $(NAME).pdf
AUX = $(NAME).aux
TEXC := xelatex
TEXC_OPTS += -shell-escape

.PHONY: clean install

all: $(PDF)

$(AUX):
	$(TEXC) $(TEXC_OPTS) $(SRC)

$(PDF):$(AUX) $(SRC)
	$(TEXC) $(TEXC_OPTS) $(SRC)
	evince $(PDF) &

clean:
	rm -f *.pdf *.aux *.log *.nav *.out *.pyg *.snm *.toc *.vrb
