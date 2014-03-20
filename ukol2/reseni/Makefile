# Autor: Martin Hruska
# E-mail: xhrusk16@stud.fit.vutbr.cz

PROJ=slo2
TEX_COMP=latex # prekladac latexu
DVI=dvips # prevod do post scriptu
A4=-t a4
PDF=ps2pdf #prevod do pdf
VLNA=vlna
VLNA_OPTS=-l -m -n

all:
	$(VLNA) $(VLNA_OPTS) $(PROJ).tex 
	$(TEX_COMP) $(PROJ).tex
	$(TEX_COMP) $(PROJ).tex
	$(DVI) $(A4) $(PROJ).dvi
	$(PDF)  $(PROJ).ps

clean:
	rm *.log *.aux *.dvi *.ps
