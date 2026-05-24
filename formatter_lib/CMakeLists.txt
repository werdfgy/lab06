cmake_minimum_required(VERSION 3.10)

# создание статической библиотеки formatter
add_library(formatter STATIC formatter.cpp)

# добавляем директорию в пути поиска заголовочных файлов
target_include_directories(formatter PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
