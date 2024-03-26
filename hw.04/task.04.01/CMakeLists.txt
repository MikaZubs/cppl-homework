cmake_minimum_required(VERSION 3.20.0)
project(LinkedListTest VERSION 0.1)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/bin)
set(SOURCE_EXE main.cpp ListNode.h LinkedList.h LinkedList.cpp)

add_executable(TSK0401 ${SOURCE_EXE})