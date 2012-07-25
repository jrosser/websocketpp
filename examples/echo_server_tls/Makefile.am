noinst_PROGRAMS = echo_server_tls

AM_CXXFLAGS = $(WSPP_CFLAGS)
LDADD = \
	$(WSPP_LIBS) \
	$(BOOST_SYSTEM_LIB) \
	$(BOOST_DATE_TIME_LIB) \
	$(BOOST_THREAD_LIB) \
	$(BOOST_REGEX_LIB) \
	$(SSL_LIBS)

echo_server_tls_SOURCES = echo.cpp echo_server_tls.cpp
noinst_HEADERS = echo.hpp
