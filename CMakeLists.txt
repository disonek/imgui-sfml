cmake_minimum_required(VERSION 3.1)

find_package(sfml REQUIRED)

add_library(imgui-sfml
   imconfig-SFML.h 
   imgui-SFML.cpp
   imgui-SFML.h
   imgui-SFML_export.h)
  
target_link_libraries(imgui-sfml PUBLIC sfml::sfml imgui)  
target_include_directories(imgui-sfml PUBLIC .)