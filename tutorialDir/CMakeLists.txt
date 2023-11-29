cmake_minimum_required(VERSION 3.0.0)
#this must be at the top to address cmake requirement
project(TestProject
		VERSION 0.0.1
		DESCRIPTION "Test for CMake Tutorial 1"
		LANGUAGES CXX)
#this describes about and project and its related information
set(CMAKE_CXX_COMPILER g++)
#set a specific compiler. This command is not required necessarily.
add_executable(TestExecutableMain main.cpp)
#this command states the name of required executable followed by source fileS
target_compile_features(TestExecutableMain PRIVATE cxx_std_20)
#this statement gives the command to utilize c++ 20 standard for the given executable compilation.