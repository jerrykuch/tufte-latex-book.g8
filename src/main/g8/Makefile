#
# We should be generating bibliography, internal references, and index
# properly. We also build the document with -synctex to enable TeXworks
# and similar tools to navigate from PDF output back to source lines.
#

base_file_name = $name$

pdf:	\$(base_file_name).tex
	pdflatex -synctex=1 -shell-escape \$(base_file_name).tex
	bibtex \$(base_file_name)
	texindy --language english \$(base_file_name).idx
# or...	makeindex \$(base_file_name)
	pdflatex -synctex=1 -shell-escape \$(base_file_name).tex
	pdflatex -synctex=1 -shell-escape \$(base_file_name).tex
	pdflatex -synctex=1 -shell-escape \$(base_file_name).tex

# Works with Mac OS X Preview.app; replace with your platform's PDF viewer
preview:	pdf
	open \$(base_file_name).pdf

.PHONY: clean
clean:
	rm -f  *.aux *.bbl *.idx *.lof *.log *.lot *.out *.pdf $(base_file_name).pdf
	rm -rf _minted-$(base_file_name)

