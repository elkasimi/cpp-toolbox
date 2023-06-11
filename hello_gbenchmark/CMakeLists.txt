cmake_minimum_required(VERSION 3.20)
project(hello_gbenchmark)

set(CMAKE_CXX_STANDARD 23)

find_package(benchmark REQUIRED)

add_executable(
  hello_gbenchmark
  hello_gbenchmark.cc
)

target_link_libraries(
  hello_gbenchmark
  benchmark::benchmark
)
