cmake_minimum_required(VERSION 3.3)

project(boost_type_index)

add_library(boost_type_index INTERFACE)

target_include_directories(boost_type_index BEFORE INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}/include)

install(TARGETS boost_type_index DESTINATION lib)
install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/include/boost DESTINATION include)
