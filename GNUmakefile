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
	cp LICENSE  $(DESTDIR)$(PREFIX)/share/doc/$(PROJECT)
## -- BLOCK:license --
## -- BLOCK:sh --
install: install-sh
install-sh:
	mkdir -p $(DESTDIR)$(PREFIX)/bin
	cp bin/run              $(DESTDIR)$(PREFIX)/bin
	cp bin/scratch          $(DESTDIR)$(PREFIX)/bin
	cp bin/trash            $(DESTDIR)$(PREFIX)/bin
	cp bin/template         $(DESTDIR)$(PREFIX)/bin
	cp bin/search-project   $(DESTDIR)$(PREFIX)/bin
	cp bin/fnote            $(DESTDIR)$(PREFIX)/bin
	cp bin/new-project      $(DESTDIR)$(PREFIX)/bin
	cp bin/trash-code       $(DESTDIR)$(PREFIX)/bin
	cp bin/pwdvar           $(DESTDIR)$(PREFIX)/bin
	cp bin/import-code      $(DESTDIR)$(PREFIX)/bin
## -- BLOCK:sh --
