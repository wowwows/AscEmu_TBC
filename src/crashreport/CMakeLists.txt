# Copyright (C) 2014-2016 AscEmu Team <http://www.ascemu.org>

project(crashreport)

set(SRCS Main.c)

add_executable(${PROJECT_NAME} ${SRCS})
install(TARGETS ${PROJECT_NAME} RUNTIME DESTINATION .)
unset(SRCS)
