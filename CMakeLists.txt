cmake_minimum_required(VERSION 4.3.4)

project(Nearby VERSION 1.0.0
        DESCRIPTION "Nearby C++ SDK"
        LANGUAGES CXX)

        
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
        
find_package(Boost REQUIRED)
target_link_libraries(nearby PRIVATE Boost::boost)

add_executable(nearby src/main.cpp)