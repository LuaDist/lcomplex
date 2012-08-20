# Copyright (C) 2007-2012 LuaDist.
# Created by Peter Kapec
# Redistribution and use of this file is allowed according to the terms of the MIT license.
# For details see the COPYRIGHT file distributed with LuaDist.
# Please note that the package source code is licensed under its own license.

project ( lcomplex C )
cmake_minimum_required ( VERSION 2.8 )
include ( cmake/dist.cmake )
include ( lua )

# Build
add_lua_module ( complex lcomplex.c )

# Install all files and documentation
install ( TARGETS complex DESTINATION ${INSTALL_CMOD} )
install ( FILES README DESTINATION ${INSTALL_DATA} )
install ( FILES test.lua DESTINATION ${INSTALL_TEST} )
