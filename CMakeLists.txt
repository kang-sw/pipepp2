cmake_minimum_required(VERSION 3.20)
project(pipepp2)

add_library(pipepp2 INTERFACE)
add_library(pipepp2::pipepp ALIAS pipepp2)

target_include_directories(pipepp2 INTERFACE include)
