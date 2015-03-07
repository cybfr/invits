INVIT = invit-ines-8ans
IMAGES = floral_border.png
all: $(INVIT).pdf $(INVIT)_enveloppe.pdf

$(INVIT).pdf: $(INVIT).tex $(IMAGES) list.csv
	xelatex -src-specials -shell-escape -interaction=nonstopmode $(INVIT).tex

$(INVIT)_enveloppe.pdf: $(INVIT)_enveloppe.tex $(IMAGES) list.csv
	xelatex -src-specials -shell-escape -interaction=nonstopmode $(INVIT)_enveloppe.tex

.PHONY: clean

clean:
	rm -f *.log *.aux *.pdf *.backup
