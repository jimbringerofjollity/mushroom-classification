# Jim Tao
# LaTeX Default Makefile

# Macros
 TEXC = pdflatex
# TEXC = 
 TEXCFLAGS = 
# TEXCFLAGS = 
 BIBTEXC = bibtex
# BIBTEXC =
 BIBTEXCFLAGS =
# BIBTEXCFLAGS =

# Dependency rules for non-file targets
all: pdf
clean: 
	rm -f *.aux *.pdf *.bbl *.blg *.log *.nav *.out *.snm *.toc
clobber: clean
	rm -f *.log

# Dependency rules for file targets
pdf: slide_deck.tex bibliography.bib
	$(TEXC) $(TEXCFLAGS) slide_deck.tex; $(BIBTEXC) $(BIBTEXCFLAGS) slide_deck.aux; $(TEXC) $(TEXCFLAGS) slide_deck.tex; $(TEXC) $(TEXCFLAGS) slide_deck.tex
