# Makefile for building C stuff with GSL
#
FILEM=tesis
FOLDER=Caps
FILE1=01_intro
TEX=pdflatex
BIBTEX=bibtex
INDEX=makeindex
VIEW=evince
FLAGS = -Wall -O3 -I/usr/local/include

FOLDER/FILE1.tex: $(FILEM).tex
	$(TEX) $(FILEM)
	$(TEX) $(FILEM)
	$(INDEX) $(FILEM).nlo -s nomencl.ist -o $(FILEM).nls
	$(BIBTEX) $(FILEM)
	$(TEX) $(FILEM)
	$(TEX) $(FILEM)
	$(VIEW) $(FILEM).pdf &

quick: $(FILEM).tex
	$(TEX) $(FILEM)
	$(VIEW) $(FILEM).pdf &


clean:
	rm -f *~ *.aux *.blg *.out *.bbl *.log *.ilg *.ind *.lof *.nlo *.nls *.toc *.dvi *.pdf
