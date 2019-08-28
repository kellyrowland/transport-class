all:
	@pdflatex intro

current_dir = $(shell pwd)

dock:
	@docker pull kellyrowland/docker-texlive
	@docker run -v $(current_dir):/doc/ \
        -t -i kellyrowland/docker-texlive

clean:
	@rm -f *.aux \
           *.bbl \
           *.bcf \
           *.blg \
           *.dvi \
           *.lof \
           *.log \
           *.lot \
           *.nav \
           *.out \
           *.snm \
           *.toc \
	       *.run.xml
