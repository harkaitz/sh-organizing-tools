PROJECT=sh-organizing-tools
VERSION=1.0.0
PREFIX=/usr/local
all:
clean:
install:

## -- BLOCK:license --
install: install-license
install-license: 
	mkdir -p $(DESTDIR)$(PREFIX)/share/doc/$(PROJECT)
	cp LICENSE README.md $(DESTDIR)$(PREFIX)/share/doc/$(PROJECT)
update: update-license
update-license:
	ssnip README.md
## -- BLOCK:license --
## -- BLOCK:sh --
install: install-sh
install-sh:
	mkdir -p $(DESTDIR)$(PREFIX)/bin
	cp bin/note             $(DESTDIR)$(PREFIX)/bin
	cp bin/run              $(DESTDIR)$(PREFIX)/bin
	cp bin/trash            $(DESTDIR)$(PREFIX)/bin
	cp bin/template         $(DESTDIR)$(PREFIX)/bin
	cp bin/trash-code       $(DESTDIR)$(PREFIX)/bin
## -- BLOCK:sh --
