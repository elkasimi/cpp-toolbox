cmake_minimum_required(VERSION 3.20)
project(hello_gtest)

# GoogleTest requires at least C++14
set(CMAKE_CXX_STANDARD 23)

find_package(GTest REQUIRED)

add_executable(
  hello_gtest
  hello_gtest.cc
)

target_link_libraries(
  hello_gtest
  GTest::gtest
  GTest::gtest_main
)

# cf. https://cmake.org/cmake/help/latest/module/FindGTest.html
