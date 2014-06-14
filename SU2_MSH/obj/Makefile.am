# SU2 Makefile.am for MAC
# Stanford University Aerospace Design Lab
#
# Created: 		10/26/12
# Last updated: 	3/12/13
#
# Created by: 		M. Colonno
# Updated by: 		M. Colonno
#
##########################

# AUTOMAKE_OPTIONS = subdir-objects
ACLOCAL_AMFLAGS = ${ACLOCAL_FLAGS}

bin_PROGRAMS = ../bin/SU2_MSH

___bin_SU2_MSH_SOURCES = ../include/SU2_MSH.hpp \
		../src/SU2_MSH.cpp

___bin_SU2_MSH_CXXFLAGS =
___bin_SU2_MSH_LDADD = ../../Common/lib/libSU2.a

# always link to built dependencies from ./externals
___bin_SU2_MSH_CXXFLAGS += @su2_externals_INCLUDES@
___bin_SU2_MSH_LDADD += @su2_externals_LIBS@

# if BUILD_CGNS
___bin_SU2_MSH_CXXFLAGS += @CGNS_CXX@
___bin_SU2_MSH_LDADD += @CGNS_LD@
# endif

# if BUILD_MUTATIONPP
___bin_SU2_MSH_CXXFLAGS += @MUTATIONPP_CXX@
___bin_SU2_MSH_LDADD += @MUTATIONPP_LD@
# endif

# if BUILD_JSONCPP
___bin_SU2_MSH_CXXFLAGS += @JSONCPP_CXX@
___bin_SU2_MSH_LDADD += @JSONCPP_LD@
# endif