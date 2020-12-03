project(Tinyhttpd)

cmake_minimum_required(VERSION 3.0)
#CMAKE_PROJECT_VERSION()
#CMAKE_PROJECT_VERSION_MAJOR()
#CMAKE_PROJECT_VERSION_MINOR()
#CMAKE_PROJECT_VERSION_PATCH()
set(CMAKE_CXX_STANDARD 11)

add_subdirectory(include/nlohmann)
add_library(httpd ...)

add_executable(httpd httpd.cpp)

target_link_libraries(httpd pthread)
target_link_libraries(httpd private nlohmann_json)

## 尝试手动链接
# g++ -o main -I./include/ httpd.cpp -lpthread