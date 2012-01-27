presentation:
	xelatex -shell-escape presentation
	bibtex presentation
	xelatex -shell-escape presentation

PHONY : clean reallyclean

clean:
	for i in log aux ps dvi bbl blg log lof lot toc out pyg glg glo gls ist; do rm -f *.$$i; done

reallyclean: clean
	rm -f *.{ps,pdf}
