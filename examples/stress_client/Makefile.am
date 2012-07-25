noinst_PROGRAMS = stress_client

AM_CXXFLAGS = $(WSPP_CFLAGS)
LDADD = \
	$(WSPP_LIBS) \
	$(BOOST_SYSTEM_LIB) \
	$(BOOST_DATE_TIME_LIB) \
	$(BOOST_THREAD_LIB) \
	$(BOOST_RANDOM_LIB) \
	$(BOOST_REGEX_LIB)

stress_client_SOURCES = stress_client.cpp
