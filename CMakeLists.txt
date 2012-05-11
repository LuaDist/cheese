# Copyright (C) 2007-2012 LuaDist.
# Created by Peter Kapec
# Redistribution and use of this file is allowed according to the terms of the MIT license.
# For details see the COPYRIGHT file distributed with LuaDist.
# Please note that the package source code is licensed under its own license.

project ( cheese NONE )
cmake_minimum_required ( VERSION 2.8 )
include ( cmake/dist.cmake )
include ( lua )

install_lua_module ( cheese src/cheese.lua )
install_lua_module ( stream.file src/stream/file.lua )
install_lua_module ( stream.string src/stream/string.lua )
install_lua_module ( cheese.parsers src/parsers.lua )
install_lua_module ( cheese.luap src/luap/luap.lua )
install_lua_module ( cheese.luap.dump src/luap/dump.lua )
install_data ( README )
install_doc ( doc/ )
install_test ( test/ )

#FIX-path: add_lua_test ( test/test.lua )
