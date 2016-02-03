CC=pdflatex

all:Report

Report:Report.tex
	$(CC) --jobname $@ $^
	makeglossaries $@
	bibtex $@
	$(CC) --jobname $@ $^
	$(CC) --jobname $@ $^
	evince $@.pdf &

Content:
	pdftk A=Report.pdf cat A2-3 output Table_of_Content.pdf

clean:
	rm -rf Table_of_Content.pdf Report.pdf *.aux *.log *.bbl *.blg *.toc
