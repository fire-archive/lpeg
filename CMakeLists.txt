# Copyright (C) 2007-2009 LuaDist.
# Created by Peter Drahoš
# Redistribution and use of this file is allowed according to the terms of the MIT license.
# For details see the COPYRIGHT file distributed with LuaDist.
# Please note that the package source code is licensed under its own license.

project(lpeg C)
cmake_minimum_required(VERSION 2.6)
include(dist.cmake)

install_lua_module(lpeg lpeg.c lpeg.def)
install_lua_module(re re.lua)
install_doc(re.html lpeg.html lpeg-128.gif)
install_test(test.lua)

add_lua_test(test.lua)
