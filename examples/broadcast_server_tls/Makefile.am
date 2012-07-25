noinst_PROGRAMS = broadcast_server

AM_CXXFLAGS = $(WSPP_CFLAGS)
LDADD = \
	$(WSPP_LIBS) \
	$(BOOST_SYSTEM_LIB) \
	$(BOOST_DATE_TIME_LIB) \
	$(BOOST_REGEX_LIB) \
	$(BOOST_THREAD_LIB) \
	$(SSL_LIBS)

broadcast_server_SOURCES = broadcast_server_tls.cpp
noinst_HEADERS = broadcast_admin_handler.hpp \
	   	 broadcast_handler.hpp \
		 broadcast_server_handler.hpp \
		 wscmd.hpp
