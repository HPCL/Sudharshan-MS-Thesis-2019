SHELL = /bin/sh

all: main.pdf

main.pdf: *.tex *.bib *.cls
	/Library/TeX/Root/bin/x86_64-darwin/pdflatex main.tex
	bibtex main
	touch main.tex
	/Library/TeX/Root/bin/x86_64-darwin/pdflatex main.tex
	/Library/TeX/Root/bin/x86_64-darwin/pdflatex main.tex

short: *.tex 
	/Library/TeX/Root/bin/x86_64-darwin/pdflatex main.tex

clean:
	if (rm -f main.pdf *.lol *.loa *.lof *.lot *.out *.log *.aux *.bbl *.blg *.toc *.dvi *.ps *.brf *.lbl) then :; fi

