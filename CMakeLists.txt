cmake_minimum_required(VERSION "3.27.4")

project("TournamentOrganiser" VERSION 1.0)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

add_executable("${PROJECT_NAME}" "TournamentOrganiser.cpp")

include(CTest)

add_test("test1" "${CMAKE_CURRENT_BINARY_DIR}/${PROJECT_NAME}")