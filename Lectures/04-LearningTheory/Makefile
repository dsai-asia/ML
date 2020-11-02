
SRC=04-Learning-Theory.tex

TARGDISP=$(SRC:.tex=.pdf)
TARGPRINT2=$(SRC:.tex=x2.pdf)
TARGPRINT4=$(SRC:.tex=x4.pdf)

all: $(TARGDISP)

$(TARGDISP): $(SRC) *.tex
	pdflatex $(SRC)

$(TARGPRINT4): $(TARGDISP)
	pdfnup --nup 2x2 --frame true --offset "0 0" --scale 0.8 \
		--delta "1cm 1cm" --outfile $(TARGPRINT4) $(TARGDISP)

$(TARGPRINT2): $(TARGDISP)
	pdfnup --nup 1x2 --frame true --offset "0 0" --scale 0.8 \
		--delta "1cm 1cm" --outfile $(TARGPRINT2) $(TARGDISP)

