noinst_PROGRAMS = telemetry_server

AM_CXXFLAGS = $(WSPP_CFLAGS)
LDADD = \
	$(WSPP_LIBS) \
	$(BOOST_SYSTEM_LIB) \
	$(BOOST_TIME_DATE_LIB) \
	$(BOOST_PROGRAM_OPTIONS_LIB) \
	$(BOOST_THREAD_LIB) \
	$(BOOST_REGEX_LIB)

telemetry_server_SOURCES = telemetry_server.cpp
