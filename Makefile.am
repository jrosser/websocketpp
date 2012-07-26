AUTOMAKE_OPTIONS = foreign

SUBDIRS = src test/basic examples

pkgconfig_DATA = websocketpp-$(WSPP_MAJORMINOR).pc

websocketpp-$(WSPP_MAJORMINOR).pc: websocketpp.pc
	        cp websocketpp.pc websocketpp-$(WSPP_MAJORMINOR).pc

BUILT_SOURCES = websocketpp-$(WSPP_MAJORMINOR).pc

CLEANFILES = websocketpp-$(WSPP_MAJORMINOR).pc

ACLOCAL_FLAGS = -I m4
