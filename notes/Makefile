SRCTYPE=markdown_github
SRCFILE=linear_regression.md
DESTTYPE=html
DESTFILE=test.html
BUILD=pandoc --from $(SRCTYPE) --to $(DESTTYPE) $(SRCFILE) > $(DESTFILE)

all:
	$(BUILD)
	open $(DESTFILE)

clean:
	rm -f $(DESTFILE)
