cmake_minimum_required(VERSION 3.4.3 FATAL_ERROR)

project(k380-function-keys-exe)

set(CMAKE_C_STANDARD 11)
add_compile_options(-Wall -Wextra -Werror)
add_executable(k380-fn-exe main.c)

target_link_libraries(k380-fn-exe PRIVATE hidapi::hidapi)
