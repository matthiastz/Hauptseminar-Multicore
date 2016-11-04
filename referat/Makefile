TMPFILES	= *.{log,aux,toc,out,lof,lot,snm,nav,vrb,pdf,bak}


default:	beamer

all:		beamer handout notes dualmon


beamer:		beamer.pdf
handout:	handout.pdf
notes:		notes.pdf
dualmon:	dualmon.pdf
article:	article.pdf


%.pdf: %.tex main.tex $(wildcard include/*) $(wildcard Grafiken/*)
	pdflatex $<
	pdflatex $<
	pdflatex $<

clean:
	rm -f $(TMPFILES)
