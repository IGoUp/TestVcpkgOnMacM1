cmake_minimum_required (VERSION 3.0.0)
project (Transformation)

find_package(Eigen3 CONFIG REQUIRED)
include_directories(/opt/homebrew/var/vcpkg/installed/arm64-osx/include)

add_executable (Transformation main.cpp)
target_link_libraries(Transformation PRIVATE Eigen3::Eigen)