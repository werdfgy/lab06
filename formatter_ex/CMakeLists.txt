cmake_minimum_required(VERSION 3.10)
project(formatter_ex)

# Создаем статическую библиотеку
add_library(formatter_ex STATIC formatter_ex.cpp)

# добавляем текущую директорию в пути поиска заголовочных файлов
target_include_directories(formatter_ex PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

# линковка с базовой библиотекой formatter
target_link_libraries(formatter_ex PUBLIC formatter)
