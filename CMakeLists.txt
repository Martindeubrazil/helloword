cmake_minimum_required(VERSION 3.16)

project(helloword LANGUAGES C)

add_executable(helloword main.c)

include(GNUInstallDirs)
install(TARGETS helloword
    LIBRARY DESTINATION ${CMAKE_INSTALL_LIBDIR}
    RUNTIME DESTINATION ${CMAKE_INSTALL_BINDIR}
)
