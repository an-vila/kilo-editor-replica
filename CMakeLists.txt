cmake_minimum_required(VERSION 3.16)

project(text_editor LANGUAGES C)

add_executable(text_editor main.c)

include(GNUInstallDirs)
install(TARGETS text_editor
    LIBRARY DESTINATION ${CMAKE_INSTALL_LIBDIR}
    RUNTIME DESTINATION ${CMAKE_INSTALL_BINDIR}
)
