# Copyright (C) 2014-2016 AscEmu Team <http://www.ascemu.org>

# set up our project name
project(dbcfile)

set(sources
   dbcfile.cpp
)

include_directories(
   ${CMAKE_SOURCE_DIR}/dep/loadlib
   ${CMAKE_SOURCE_DIR}/dep/libmpq/libmpq
   ${CMAKE_CURRENT_SOURCE_DIR}
)

add_library(${PROJECT_NAME} STATIC ${sources})
target_link_libraries( ${PROJECT_NAME} loadlib libmpq)

unset(sources)
