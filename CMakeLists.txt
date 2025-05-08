cmake_minimum_required(VERSION 3.16)

project(boost-headers-only
    VERSION 1.87.0
    LANGUAGES CXX
)

add_library(boost-headers-only INTERFACE)

target_include_directories(boost-headers-only INTERFACE
    ${CMAKE_CURRENT_SOURCE_DIR}
)

set_target_properties(boost-headers-only PROPERTIES
    INTERFACE_INCLUDE_DIRECTORIES ${CMAKE_CURRENT_SOURCE_DIR}
)
