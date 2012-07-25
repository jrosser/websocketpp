noinst_PROGRAMS = tests perf

AM_CXXFLAGS = $(WSPP_CFLAGS)
LDADD = \
	$(WSPP_LIBS) \
	$(BOOST_UNIT_TEST_FRAMEWORK_LIB) \
	$(BOOST_SYSTEM_LIB) \
	$(BOOST_RANDOM_LIB)

tests_SOURCES = hybi_util.cpp

perf_SOURCES = uri_perf.cpp
