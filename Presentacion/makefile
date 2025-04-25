# Makefile for generating presentation $(TARGET).pdf from $(TARGET).tex 

TARGET = example

all: $(TARGET).pdf

$(TARGET).pdf: $(TARGET)-tmp.pdf
	ppower4 $(TARGET)-tmp.pdf $(TARGET).pdf

$(TARGET)-tmp.pdf: $(TARGET).tex
	pdflatex $(TARGET).tex
	mv $(TARGET).pdf $(TARGET)-tmp.pdf

clean:
	rm -f $(TARGET).pdf $(TARGET)-tmp.pdf $(TARGET).log $(TARGET).aux

