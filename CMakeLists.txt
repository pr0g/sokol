cmake_minimum_required(VERSION 3.15)
project(sokol LANGUAGES C)
add_library(${PROJECT_NAME} INTERFACE)
target_include_directories(
    ${PROJECT_NAME}
    INTERFACE $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}>)
target_compile_features(${PROJECT_NAME} INTERFACE c_std_99)
