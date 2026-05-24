cmake_minimum_required(VERSION 3.10)
project(FormatterIncProject)

# устанавливаем стандарт C++
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(PRINT_VERSION_MAJOR 0)
set(PRINT_VERSION_MINOR 1)
set(PRINT_VERSION_PATCH 0)
set(PRINT_VERSION_TWEAK 0)
set(PRINT_VERSION $PRINT_VERSION_MAJOR.$PRINT_VERSION_MINOR.$PRINT_VERSION_PATCH.$PRINT_VERSION_TWEAK)

include(CPackConfig.cmake)

# добавляем поддиректории(в порядке зависимостей)
add_subdirectory(formatter_lib)

add_subdirectory(formatter_ex)

add_subdirectory(hello_world)

add_subdirectory(solver_lib)

add_subdirectory(solver)
