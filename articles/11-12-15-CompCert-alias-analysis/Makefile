report:
	rm -f report.glo report.glg report.gls
	xelatex -shell-escape report
	bibtex report
	makeglossaries report
	xelatex -shell-escape report
	makeglossaries report
	xelatex -shell-escape report

PHONY : clean reallyclean

clean:
	for i in log aux ps dvi bbl blg log lof lot toc out pyg glg glo gls ist; \
		do rm -f *.$$i; done

reallyclean: clean
	rm -f *.{ps,pdf}
