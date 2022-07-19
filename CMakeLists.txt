cmake_minimum_required(VERSION 3.22)
project(PocoTest)

set(CMAKE_CXX_STANDARD 14)

find_package(Poco COMPONENTS Data REQUIRED)
add_executable(PocoTest main.cpp)
target_link_libraries(PocoTest PRIVATE Poco::Data)
