AUTOMAKE_OPTIONS = foreign no-dependencies

INCLUDES = -I..

noinst_LIBRARIES = libdb.a
libdb_a_SOURCES = \
   blockfile.cpp blockrecordarray.cpp blockrecordfile.cpp 	\
   db.cpp hierdatabase.cpp hierdbpath.cpp stddb.cpp
 
DEFS = @DEFS@		# This gets rid of the -I. so INCLUDES must be more explicit

all: $(noinst_LIBRARIES)
	$(AR) ru ../../lib/libtripwire.a $(libdb_a_OBJECTS)
