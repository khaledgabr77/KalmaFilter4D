project(KalmanFilter)

cmake_minimum_required (VERSION 3.5)

add_definitions(-std=c++11)

set(CXX_FLAGS "-Wall")
set(CMAKE_CXX_FLAGS "${CXX_FLAGS}")

set(sources main.cpp tracking.cpp  tracking.h measurements_package.h kalman_filter.h
    kalman_filter.cpp )



add_executable(KalmanFilter ${sources})

target_link_libraries(KalmanFilter)