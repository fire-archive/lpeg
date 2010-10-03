# Copyright (C) 2007-2009 LuaDist.
# Created by Peter Drahoš
# Redistribution and use of this file is allowed according to the terms of the MIT license.
# For details see the COPYRIGHT file distributed with LuaDist.
# Please note that the package source code is licensed under its own license.

PROJECT(lpeg C)
CMAKE_MINIMUM_REQUIRED(VERSION 2.6)
INCLUDE(dist.cmake)

ADD_LUA_MODULE(lpeg lpeg.c lpeg.def)
ADD_LUA_TEST(test.lua)

INSTALL(TARGETS lpeg DESTINATION ${INSTALL_CMOD})
INSTALL(FILES re.lua DESTINATION ${INSTALL_LMOD})
INSTALL(FILES re.html lpeg.html lpeg-128.gif DESTINATION ${INSTALL_DOC})
INSTALL(FILES test.lua DESTINATION ${INSTALL_TEST})
