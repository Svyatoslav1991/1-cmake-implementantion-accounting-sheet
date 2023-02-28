cmake_minimum_required(VERSION 3.15)
project("1_implementantion_accounting_sheet" VERSION 1.0)

set(CMAKE_CXX_STANDARD 14)

add_executable(1_implementantion_accounting_sheet include/employer.h include/functions.h src/main.cpp src/functions.cpp statement.txt)
target_include_directories(1_implementantion_accounting_sheet PUBLIC include)
configure_file(statement.txt ${CMAKE_CURRENT_BINARY_DIR}/statement.txt COPYONLY)