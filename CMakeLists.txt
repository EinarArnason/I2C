cmake_minimum_required(VERSION 3.0.0)
project(I2C VERSION 0.1.0)

include(CTest)
enable_testing()

add_library(${PROJECT_NAME} INTERFACE)
target_include_directories(${PROJECT_NAME} INTERFACE ${PROJECT_SOURCE_DIR}/include)

target_compile_features(${PROJECT_NAME} INTERFACE cxx_std_17)

set(CPACK_PROJECT_NAME ${PROJECT_NAME}) 
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
