cmake_minimum_required(VERSION 3.10 FATAL_ERROR)
# tell CMake not to define WIN32 when building with Cygwin
set(CMAKE_LEGACY_CYGWIN_WIN32 0)

# set the project name
project(Test VERSION 1.0)

# specify the C++ standard
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

include_directories(${CMAKE_CURRENT_SOURCE_DIR})
add_subdirectory(TestCore)

# add the executable
add_executable(test main.cpp)
target_link_libraries(test TestCore)

# install(TARGETS test DESTINATION /some/full/path)
