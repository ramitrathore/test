#cmake_minimum_required(VERSION 3.8)

project (hello-cmake)

add_subdirectory(test)

add_executable(hello hello.cpp)

target_link_libraries(
    hello
    PRIVATE test 
)


install(TARGETS hello DESTINATION hello/bin)