cmake_minimum_required(VERSION 3.10)

project(HelloWorld)

# add_subdirectory(fmt)
# include(d:/vcpkg/scripts/buildsystems/vcpkg.cmake)

find_package(fmt CONFIG REQUIRED)
# find_package(DataFrame CONFIG REQUIRED)

add_executable(HelloWorld helloworld.cpp)

target_link_libraries(HelloWorld PRIVATE fmt::fmt)

