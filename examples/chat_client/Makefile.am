noinst_PROGRAMS = chat_client

AM_CXXFLAGS = $(WSPP_CFLAGS)
LDADD = \
	$(WSPP_LIBS) \
	$(BOOST_SYSTEM_LIB) \
	$(BOOST_THREAD_LIB) \
	$(BOOST_RANDOM_LIB)

chat_client_SOURCES = chat_client.cpp chat_client_handler.cpp
noinst_HEADERS = chat_client_handler.hpp
