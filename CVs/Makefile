SRCS:=$(wildcard *.tex)
RES:=$(patsubst %.tex,%.pdf,$(SRCS))

all: $(RES)

%.pdf: %.tex
	@pdflatex $<

clean:
	@rm -f *.pdf
	@rm -f *.out
	@rm -f *.aux
	@rm -f *.log
