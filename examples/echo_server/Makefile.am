noinst_PROGRAMS = echo_server

AM_CXXFLAGS = $(WSPP_CFLAGS)
LDADD = \
	$(WSPP_LIBS) \
	$(BOOST_PROGRAM_OPTIONS_LIB) \
	$(BOOST_SYSTEM_LIB) \
	$(BOOST_THREAD_LIB)

echo_server_SOURCES = echo_server.cpp
