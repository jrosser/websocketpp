noinst_PROGRAMS = fuzzing_client

AM_CXXFLAGS = $(WSPP_CFLAGS)
LDADD = \
	$(WSPP_LIBS) \
	$(BOOST_SYSTEM_LIB) \
	$(BOOST_RANDOM_LIB)

fuzzing_client_SOURCES = fuzzing_client.cpp
