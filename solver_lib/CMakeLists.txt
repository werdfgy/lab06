cmake_minimum_required(VERSION 3.10)
project(solver_lib)

# создаем статическую библиотеку
add_library(solver_lib STATIC solver.cpp)

# добавляем текущую директорию в пути поиска заголовочных файлов
target_include_directories(solver_lib PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
