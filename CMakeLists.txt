cmake_minimum_required(VERSION 3.5)
project(usefull)

# Do not allow in-source builds:
if (CMAKE_SOURCE_DIR STREQUAL CMAKE_BINARY_DIR)
    message(FATAL_ERROR "In-source builds are not allowed.")
endif()

install(DIRECTORY bin/ DESTINATION ${CMAKE_INSTALL_PREFIX}/bin USE_SOURCE_PERMISSIONS)
