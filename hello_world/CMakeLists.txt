cmake_minimum_required(VERSION 3.10)
project(hello_world)

# Создаем исполняемый файл
# Путь к файлу можно указать относительно текущей директории
add_executable(hello_world hello_world.cpp)

# Линковка с библиотекой formatter_ex
# PRIVATE - так как приложение не экспортирует зависимости наружу
target_link_libraries(hello_world PRIVATE formatter_ex)
