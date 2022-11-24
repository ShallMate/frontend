cmake_minimum_required(VERSION 3.15)
project(Test)

add_executable(main main.cpp util.cpp)

find_package(libOTe REQUIRED)

#target_compile_options(main PRIVATE $<$<COMPILE_LANGUAGE:CXX>:-std=c++14> -pthread)

target_link_libraries(main oc::libOTe)