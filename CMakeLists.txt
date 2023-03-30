cmake_minimum_required(VERSION 3.24)
project(openroad-embedding)

set(CMAKE_CXX_STANDARD 17)

add_executable(openroad-embedding main.cpp)

add_subdirectory(submodule/OpenROAD)

target_link_libraries(openroad-embedding
        PUBLIC
        odb
        mpl2_lib
        )