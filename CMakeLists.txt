cmake_minimum_required(VERSION 3.12)  # Minimum version of CMake

# Set the project name and version
project(InCabinMonitoring VERSION 1.0.0)

# C++ Standard
set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# Find OpenCV
find_package(OpenCV REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS})

# Find TensorFlow
find_package(TensorFlow REQUIRED)
include_directories(${TensorFlow_INCLUDE_DIRS})

# Specify include directory
include_directories(include)

# Add your source directory
add_subdirectory(src)

# Specify the target
add_executable(InCabinMonitoring main.cpp)

# Link the libraries to your project
target_link_libraries(InCabinMonitoring ${OpenCV_LIBS} ${TensorFlow_LIBS})

