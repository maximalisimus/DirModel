cmake_minimum_required(VERSION 3.2)

project(DirModel)

set(CMAKE_AUTOMOC ON)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

if(${CMAKE_SYSTEM_NAME} STREQUAL Windows)
	set(CC "gcc")
	set(CXX "g++")
	set(CMAKE_GENERATOR "Unix Makefiles")
endif()

find_package(Qt5Widgets REQUIRED)
find_package(Qt5 COMPONENTS Gui REQUIRED)
find_package(Qt5 COMPONENTS Core REQUIRED)

add_executable(DirModel main.cpp)

qt5_use_modules(DirModel Widgets Gui Core)
