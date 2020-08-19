
SRC=01-Introduction.tex

TARGDISP=$(SRC:.tex=.pdf)

all: $(TARGDISP)

$(TARGDISP): $(SRC) *.tex
	pdflatex $(SRC)
	pdflatex $(SRC)

clean:
	rm -f $(TARGDISP) *.aux *.toc *.vrb *.log *.nav *.snm *.out
