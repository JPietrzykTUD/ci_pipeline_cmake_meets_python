cmake_minimum_required(VERSION 3.15)
project(TEST)


set(Python_FIND_VIRTUALENV FIRST)
find_package(Python3 REQUIRED)

message(STATUS "${PYTHON3_EXECUTABLE}")
message(STATUS "${VIRTUALENV}")

execute_process(
        COMMAND "${Python3_EXECUTABLE} main.py"
)
