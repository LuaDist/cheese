# Copyright (C) 2007-2009 LuaDist.
# Created by Peter Kapec
# Redistribution and use of this file is allowed according to the terms of the MIT license.
# For details see the COPYRIGHT file distributed with LuaDist.
# Please note that the package source code is licensed under its own license.

PROJECT(cheese NONE)
CMAKE_MINIMUM_REQUIRED(VERSION 2.6)
INCLUDE(dist.cmake)

# Cheese modules
INSTALL (FILES src/cheese.lua DESTINATION ${INSTALL_LMOD})
INSTALL (FILES src/stream/file.lua src/stream/string.lua DESTINATION ${INSTALL_LMOD}/stream)
INSTALL (FILES src/parsers.lua src/luap/luap.lua DESTINATION ${INSTALL_LMOD}/cheese)
INSTALL (FILES src/luap/dump.lua DESTINATION ${INSTALL_LMOD}/cheese/luap)
INSTALL (FILES README DESTINATION ${INSTALL_DATA})
INSTALL (DIRECTORY doc/ DESTINATION ${INSTALL_DOC})
INSTALL (DIRECTORY test/ DESTINATION ${INSTALL_TEST})
