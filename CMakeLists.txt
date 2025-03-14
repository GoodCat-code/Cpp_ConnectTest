cmake_minimum_required(VERSION 3.3)
project(Connect_test)

set(CMAKE_CXX_STANDARD 17)

set(XLNT_DIR "E:/C++ projects/Cpp_libs/XLNT")

include_directories(${XLNT_DIR}/include)
link_directories(${XLNT_DIR}/build/source/Release)

add_executable(Connect_test main.cpp)

target_link_libraries(Connect_test xlnt)