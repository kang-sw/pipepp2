cmake_minimum_required(VERSION 3.20)
project(pipepp2)

add_subdirectory(third/templates)
add_subdirectory(third/cppmarkup)

add_library(pipepp2 INTERFACE)
add_library(kangsw::pipepp2 ALIAS pipepp2)

target_include_directories(pipepp2 INTERFACE include)
target_link_libraries(pipepp2 INTERFACE kangsw::templates kangsw::cppmarkup)
