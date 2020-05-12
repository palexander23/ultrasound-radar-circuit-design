CONTENT = 	content/SystemBlockDiagram.tex\
			content/Specification.tex\
			content/Implementation.tex\
			content/CriticalAnalysis.tex

Report.pdf: Report.tex $(CONTENT)
	@echo "" | pdflatex Report.tex
	# @echo "" | bibtex Report.tex
	@echo "" | pdflatex Report.tex
	@echo "" | pdflatex Report.tex

clean:
	rm -r *.aux *.bcf *.log *.out *.pdf *.toc *.xml
