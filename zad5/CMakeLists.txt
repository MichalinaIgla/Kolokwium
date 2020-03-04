cmake_minimum_required(VERSION 2.8.9)
#Project name
project(myProgram)

#Heders *.h
include_directories(include)

#Sources
#set(src/address.cpp src/employee.cpp src/main.cpp )
file(GLOB SOURCES "src/*.cpp")


add_executable(myProgram ${SOURCES})
#install(TARGETS myProgram DESTINATION /temp )
 
