SUBDIRS = resources

AM_CPPFLAGS = $(WX_CXXFLAGS) \
		-I$(top_srcdir)/src/include \
		-I$(top_srcdir)/src/sdk/wxscintilla/include

pluginlibdir = $(pkglibdir)/plugins

pluginlib_LTLIBRARIES = libSymTab.la

libSymTab_la_LDFLAGS = @MODULE_SHARED_LDFLAGS@ -version-info 0:1:0 -no-undefined -avoid-version

libSymTab_la_LIBADD = ../../../sdk/libcodeblocks.la $(WX_LIBS)

libSymTab_la_SOURCES = symtabconfig.cpp \
			symtab.cpp \
			symtabexec.cpp

noinst_HEADERS = symtabconfig.h \
			symtabexec.h \
			symtab.h

EXTRA_DIST = $(srcdir)/*.cbp
