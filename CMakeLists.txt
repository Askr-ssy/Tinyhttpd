project(Tinyhttpd)

cmake_minimum_required(VERSION 3.0)
#CMAKE_PROJECT_VERSION()
#CMAKE_PROJECT_VERSION_MAJOR()
#CMAKE_PROJECT_VERSION_MINOR()
#CMAKE_PROJECT_VERSION_PATCH()
set(CMAKE_CXX_STANDARD 11)

include_directories("./include")
#add_executable(httpd httpd.cpp)
add_executable(test connmysql.cpp)

target_link_libraries(test mysqlcppconn)
#find_package("mysql")
#target_link_libraries(httpd pthread)

#target_link_libraries(httpd private nlohmann_json)

## 尝试手动链接
# g++ -o main -I./include/ httpd.cpp -lpthread