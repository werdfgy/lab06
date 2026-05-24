cmake_minimum_required(VERSION 3.10)
project(solver)

# создаем исполняемый файл
add_executable(solver equation.cpp)

# линковка с библиотеками formatter_ex и solver_lib
target_link_libraries(solver PRIVATE formatter_ex solver_lib)
