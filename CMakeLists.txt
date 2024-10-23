cmake_minimum_required(VERSION 3.16)

project(matrix_using_malloc LANGUAGES C)

add_executable(matrix_using_malloc main.c)

include(GNUInstallDirs)
install(TARGETS matrix_using_malloc
    LIBRARY DESTINATION ${CMAKE_INSTALL_LIBDIR}
    RUNTIME DESTINATION ${CMAKE_INSTALL_BINDIR}
)
