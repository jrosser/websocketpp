noinst_PROGRAMS = fuzzing_server_tls

AM_CXXFLAGS = $(WSPP_CFLAGS)
LDADD = \
	$(WSPP_LIBS) \
	$(BOOST_SYSTEM_LIB) \
	$(BOOST_DATE_TIME_LIB) \
	$(BOOST_REGEX_LIB) \
	$(BOOST_THREAD_LIB) \
	$(SSL_LIBS)

fuzzing_server_tls_SOURCES = fuzzing_server_tls.cpp
