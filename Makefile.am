
CONFIGDIR = @CONFDIR@
cicapmoduledir=@MODSDIR@
HAVE_TEMPLATE=@HAVE_TEMPLATE@
HAVE_ARCHIVE=@HAVE_ARCHIVE@
HAVE_HASALLDATA=@HAVE_HASALLDATA@

SUBDIRS = . src etc

DISTCLEANFILES = stamp-h stamp-h[0-9]*
EXTRA_DIST = \
	ChangeLog \
	COPYING \
	INSTALL \
	README \
	bootstrap.sh

DEFAULT_PREFIX          = $(prefix)
DEFAULT_CONFIG_FILE     = $(CONFIGDIR)/squidclamav.conf
DEFAULT_DOC_DIR         = $(datadir)/squidclamav
DEFAULT_LIBEXEC_DIR     = $(libexecdir)/squidclamav

DEFS = @DEFS@
OBJDIR = @OBJDIR@

man1_MANS = doc/squidclamav.1
docdir = $(DEFAULT_DOC_DIR)
doc_DATA = doc/README

install-data-local: install-docDATA
	$(mkinstalldirs) $(DESTDIR)$(DEFAULT_DOC_DIR)
	$(mkinstalldirs) $(DESTDIR)$(DEFAULT_LIBEXEC_DIR)
	$(mkinstalldirs) $(DESTDIR)$(DEFAULT_CONFIG_DIR)
	cp cgi-bin/* $(DESTDIR)$(DEFAULT_LIBEXEC_DIR)

