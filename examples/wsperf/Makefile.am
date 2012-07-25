noinst_PROGRAMS = wsperf

AM_CXXFLAGS = $(WSPP_CFLAGS)
LDADD = $(WSPP_LIBS) \
	$(BOOST_SYSTEM_LIB) \
	$(BOOST_DATE_TIME_LIB) \
	$(BOOST_REGEX_LIB) \
	$(BOOST_THREAD_LIB) \
	$(BOOST_RANDOM_LIB) \
	$(BOOST_PROGRAM_OPTIONS_LIB) \
	$(BOOST_CHRONO_LIB)

wsperf_SOURCES = case.cpp \
		 generic.cpp \
		 request.cpp \
		 stress_aggregate.cpp \
		 stress_handler.cpp \
		 wscmd.cpp \
		 wsperf.cpp

noinst_HEADERS = case.hpp \
		 generic.hpp \
		 request.hpp \
		 stress_aggregate.hpp \
		 stress_handler.hpp \
		 wscmd.hpp

