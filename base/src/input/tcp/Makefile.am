pluginsdir = $(pkgdatadir)/plugins
AM_CPPFLAGS += -I$(top_srcdir)/headers $(TLS_CPPFLAGS)
AM_CFLAGS += $(TLS_CFLAGS)

plugins_LTLIBRARIES = ipfixcol-tcp-input.la
ipfixcol_tcp_input_la_LDFLAGS = -module -avoid-version -shared
ipfixcol_tcp_input_la_LIBADD = $(TLS_LIBS) -lrt

ipfixcol_tcp_input_la_SOURCES = tcp_input.c convert.c convert.h sflow.c sflow.h sflowtool.h
