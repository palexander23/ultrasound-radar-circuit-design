CONTENT = 	content/SystemBlockDiagram.tex\
			content/Specification.tex\
			content/Implementation.tex\
			content/CriticalAnalysis.tex

Report.pdf: Report.tex $(CONTENT) Biblo.bib
	@echo "" | pdflatex Report
	@echo "" | biber Report
	@echo "" | pdflatex Report
	@echo "" | pdflatex Report
	make wordCount
clean:
	-rm -r *.aux *.bcf *.log *.out *.pdf *.toc *.xml *.bbl *.blg
	-rm -r ./content/*.aux

wordCount:
	@echo "Word Count: \c"
	@texcount -inc -1 -sum Report.tex