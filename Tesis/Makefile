# Makefile for building C stuff with GSL
#
FILEM=tesis
FILE1=01_intro
TEX=pdflatex
BIBTEX=bibtex
VIEW=okular
FLAGS = -Wall -O3 -I/usr/local/include

$(FILEM).pdf: $(FILEM).tex
	$(TEX) $(FILEM)
	$(TEX) $(FILEM)
	# $(BIBTEX) $(FILEM)
	$(TEX) $(FILEM)
	$(TEX) $(FILEM)
	$(VIEW) $(FILEM).pdf

clean:
	rm -f *~ *.aux *.blg *.out *.bbl *.log
