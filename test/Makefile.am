if WANT_LIBSDBUSPLUS

AM_CPPFLAGS = -I$(top_srcdir)
check_PROGRAMS =

TESTS = $(check_PROGRAMS)

check_PROGRAMS += message_append
message_append_CXXFLAGS = $(SYSTEMD_CFLAGS) $(PTHREAD_CFLAGS)
message_append_LDFLAGS = $(SYSTEMD_LIBS) $(PTHREAD_LIBS)
message_append_SOURCES = message/append.cpp

check_PROGRAMS += message_read
message_read_CXXFLAGS = $(SYSTEMD_CFLAGS) $(PTHREAD_CFLAGS)
message_read_LDFLAGS = $(SYSTEMD_LIBS) $(PTHREAD_LIBS)
message_read_SOURCES = message/read.cpp

check_PROGRAMS += message_types
message_types_SOURCES = message/types.cpp

check_PROGRAMS += utility_tuple_to_array
utility_tuple_to_array_SOURCES = utility/tuple_to_array.cpp

check_PROGRAMS += utility_type_traits
utility_type_traits_SOURCES = utility/type_traits.cpp

check_PROGRAMS += vtable_vtable
vtable_vtable_SOURCES = vtable/vtable.cpp vtable/vtable_c.c

endif
