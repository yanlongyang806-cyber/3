
cmake_minimum_required(VERSION 3.15)
project(veh_patch LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_WINDOWS_EXPORT_ALL_SYMBOLS ON)

# 生成两个 DLL
add_library(veh_patch_basic SHARED src/veh_patch_basic.cpp)
add_library(veh_patch_smart SHARED src/veh_patch_smart.cpp)
