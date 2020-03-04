cmake_minimum_required(VERSION 2.8.9)
project(myProgram)
set(CMAKE_BUILD_TYPE Release)

#Headers *.h
include_directories(include)

#Sources
file(GLOB SOURCES "src/*.cpp")

#add_executable(testStudent ${SOURCES})
add_library(Student SHARED ${SOURCES})
install(TARGETS Student DESTINATION /bin)


