pkgincludedir = $(includedir)/websocketpp-@WSPP_MAJORMINOR@/websocketpp

lib_LTLIBRARIES = libwebsocketpp-@WSPP_MAJORMINOR@.la

libwebsocketpp_@WSPP_MAJORMINOR@_la_LIBADD = \
	$(BOOST_TIME_DATE_LIB) \
	$(BOOST_PROGRAM_OPTIONS_LIB) \
	$(BOOST_REGEX_LIB) \
	$(BOOST_SYSTEM_LIB) \
	$(BOOST_THREAD_LIB) \
	$(BOOST_RANDOM_LIB)

libwebsocketpp_@WSPP_MAJORMINOR@_la_LDFLAGS = \
	-no-undefined \
	-version-info $(WSPP_LIBVERSION)

libwebsocketpp_@WSPP_MAJORMINOR@_la_CPPFLAGS = \
	$(BOOST_CPPFLAGS)

libwebsocketpp_@WSPP_MAJORMINOR@_la_SOURCES = \
	network_utilities.cpp \
	uri.cpp \
	base64/base64.cpp \
	md5/md5.c \
	messages/data.cpp \
	processors/hybi_header.cpp \
	processors/hybi_util.cpp \
	rng/blank_rng.cpp \
	rng/boost_rng.cpp \
	sha1/sha1.cpp

nodist_pkginclude_HEADERS = websocketpp-stdint.h
DISTCLEANFILES = websocketpp-stdint.h

nobase_pkginclude_HEADERS = \
	http/constants.hpp \
	http/parser.hpp \
	base64/base64.h \
	logger/logger.hpp \
	messages/data.hpp \
	messages/control.hpp \
	md5/md5.h \
	md5/md5.hpp \
	processors/hybi.hpp \
	processors/hybi_header.hpp \
	processors/hybi_legacy.hpp \
	processors/hybi_util.hpp \
	processors/processor.hpp \
	rng/blank_rng.hpp \
	rng/boost_rng.hpp \
	roles/client.hpp \
	roles/server.hpp \
	sha1/sha1.h \
	sockets/plain.hpp \
	sockets/socket_base.hpp \
	sockets/tls.hpp

pkginclude_HEADERS = \
        common.hpp \
	connection.hpp \
	endpoint.hpp \
	network_utilities.hpp \
	shared_const_buffer.hpp \
	uri.hpp \
	websocket_frame.hpp \
	websocketpp.hpp \
	utf8_validator/utf8_validator.hpp
