noinst_PROGRAMS = chat_server

AM_CXXFLAGS = $(WSPP_CFLAGS)
LDADD = \
	$(WSPP_LIBS) \
	$(BOOST_PROGRAM_OPTIONS_LIB) \
	$(BOOST_SYSTEM_LIB) \
	$(BOOST_THREAD_LIB)

chat_server_SOURCES = chat.cpp chat_server.cpp
noinst_HEADERS = chat.hpp
