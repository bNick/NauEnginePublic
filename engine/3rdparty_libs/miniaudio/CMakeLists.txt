cmake_minimum_required(VERSION 3.16)

project(miniaudio LANGUAGES CXX)

set(TargetName miniaudio)

add_library(${TargetName} INTERFACE)
nau_install(miniaudio core)
target_include_directories(${TargetName} INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}/)
