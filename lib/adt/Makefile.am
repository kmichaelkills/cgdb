AM_CXXFLAGS = -I$(top_srcdir)/lib/util

noinst_LIBRARIES = libadt.a

libadt_a_SOURCES = \
    std_list.cpp \
    std_list.h \
    std_types.h

# Installs the driver programs into progs directory
noinst_PROGRAMS = std_list_driver

# This is the linked list driver
std_list_driver_LDFLAGS = -L. -L$(top_builddir)/lib/util
std_list_driver_LDADD = \
libadt.a \
$(top_builddir)/lib/util/libcgdbutil.a
std_list_driver_SOURCES = std_list_driver.cpp
std_list_driver_CXXFLAGS = $(AM_CXXFLAGS)
