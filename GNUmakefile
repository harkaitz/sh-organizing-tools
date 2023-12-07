PROJECT=sh-organizing-tools
VERSION=1.0.0
PREFIX=/usr/local
all:
clean:
install:

## -- BLOCK:license --
install: install-license
install-license: 
	install -D -t $(DESTDIR)$(PREFIX)/share/doc/$(PROJECT) LICENSE
## -- BLOCK:license --
## -- BLOCK:sh --
install: install-sh
install-sh:
	mkdir -p $(DESTDIR)$(PREFIX)/bin
	cp bin/run              $(DESTDIR)$(PREFIX)/bin
	cp bin/make-h           $(DESTDIR)$(PREFIX)/bin
	cp bin/orgcompat        $(DESTDIR)$(PREFIX)/bin
	cp bin/chad             $(DESTDIR)$(PREFIX)/bin
	cp bin/trash            $(DESTDIR)$(PREFIX)/bin
	cp bin/template         $(DESTDIR)$(PREFIX)/bin
	cp bin/mailctl          $(DESTDIR)$(PREFIX)/bin
	cp bin/search-project   $(DESTDIR)$(PREFIX)/bin
	cp bin/new-project      $(DESTDIR)$(PREFIX)/bin
	cp bin/trash-code       $(DESTDIR)$(PREFIX)/bin
	cp bin/pwdvar           $(DESTDIR)$(PREFIX)/bin
	cp bin/import-code      $(DESTDIR)$(PREFIX)/bin
	cp bin/json-cfg         $(DESTDIR)$(PREFIX)/bin
	cp bin/github-h         $(DESTDIR)$(PREFIX)/bin
## -- BLOCK:sh --
