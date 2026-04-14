cmake_minimum_required(VERSION 3.10)
project(boost_wrapper LANGUAGES CXX)

add_library(store-boost INTERFACE)
target_include_directories(store-boost INTERFACE "${CMAKE_CURRENT_SOURCE_DIR}")
target_compile_definitions(store-boost INTERFACE BOOST_ALL_NO_LIB)

set(BOOST_INCLUDE_DIRS "${CMAKE_CURRENT_SOURCE_DIR}" PARENT_SCOPE)