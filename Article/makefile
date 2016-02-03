CC=pdflatex

all:High-Level_Optimization_Driven_by_Statement_Profiling

High-Level_Optimization_Driven_by_Statement_Profiling:article.tex
	$(CC) --jobname $@ $^
	#bibtex $@
	#$(CC) --jobname $@ $^
	#$(CC) --jobname $@ $^
	evince $@.pdf &


clean:
	rm -rf High-Level_Optimization_Driven_by_Statement_Profiling.pdf *.aux *.log *.bbl *.blg *.toc
