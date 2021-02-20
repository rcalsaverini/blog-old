all: circle-of-fifths.pdf clean

circle-of-fifths.pdf: circle-of-fifths.tex
	latexmk circle-of-fifths.tex --pdf

clean:
	rm *.aux *.fdb_latexmk *.log *.fls *.synctex.gz *.dvi __latexindent_temp.tex

