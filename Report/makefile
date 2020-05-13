CONTENT = 	content/SystemBlockDiagram.tex\
			content/Specification.tex\
			content/Implementation.tex\
			content/CriticalAnalysis.tex

Report.pdf: Report.tex $(CONTENT)
	@echo "" | pdflatex Report.tex
	# @echo "" | bibtex Report.tex
	@echo "" | pdflatex Report.tex
	@echo "" | pdflatex Report.tex
	make wordCount
clean:
	rm -r *.aux *.bcf *.log *.out *.pdf *.toc *.xml

wordCount:
	@echo "Word Count: \c"
	@texcount -inc -1 -sum Report.tex