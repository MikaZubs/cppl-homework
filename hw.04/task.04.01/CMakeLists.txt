cmake_minimum_required(VERSION 3.20.0)
project(TSK0401 VERSION 0.3)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/bin)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/lib ${CMAKE_CURRENT_SOURCE_DIR}/src)
add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/lib)
add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/src)

set(SOURCE_EXE ${CMAKE_CURRENT_SOURCE_DIR}/src/main.cpp)

add_executable(TSK0401 ${SOURCE_EXE})
target_link_libraries(TSK0401 LLLIB)