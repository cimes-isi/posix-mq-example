cmake_minimum_required(VERSION 2.8.5)

project(posix-mq-example)
set(PROJECT_VERSION 0.1.0)

set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wall -std=gnu99")

find_package(Threads REQUIRED)
find_library(LIBRT rt)

add_executable(${PROJECT_NAME} main.c)
target_link_libraries(${PROJECT_NAME} ${CMAKE_THREAD_LIBS_INIT} ${LIBRT})
