cmake_minimum_required(VERSION 3.5)
project(app
        VERSION 0.0.1
        DESCRIPTION "app template"
        LANGUAGES CXX)  

file(GLOB_RECURSE SOURCE_FILES src/*.cpp)
add_executable(app main.cpp ${SOURCE_FILES})

target_include_directories(app PRIVATE ${CMAKE_CURRENT_SOURCE_DIR}/include)
