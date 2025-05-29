DIA_FILES=$(wildcard *.dia)
PNG_FILES=$(DIA_FILES:.dia=.png)

DIA = dia

all: $(PNG_FILES)

%.png: %.dia
	$(DIA) --export $@  $^

.phony: clean

clean:
	rm -f $(PNG_FILES)
