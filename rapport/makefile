CC=pdflatex

all:Report

Report:Report.tex
	$(CC) --jobname $@ $^
	bibtex $@
	$(CC) --jobname $@ $^
	$(CC) --jobname $@ $^
	evince $@.pdf &

clean:
	rm -rf Report.pdf *.aux *.log *.bbl *.blg
