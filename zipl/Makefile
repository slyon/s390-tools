# Common definitions
include ../common.mak

all:
	$(MAKE) -C boot
	$(MAKE) -C src

install: all
	$(MAKE) -C src install
	$(MAKE) -C man install
	$(INSTALL) -g $(GROUP) -o $(OWNER) -m 644 doc/zipl.conf.minimal  $(DESTDIR)$(TOOLS_LIBDIR)/zipl.conf

clean:
	$(MAKE) -C src clean
	$(MAKE) -C boot clean
