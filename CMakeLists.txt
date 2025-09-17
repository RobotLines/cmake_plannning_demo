cmake_minimum_required(VERSION 3.29.0)
project(planning
    VERSION 0.01
    DESCRIPTION "a demo of cmake planning"
    HOMEPAGE_URL "git@github.com:RobotLines/cmake_plannning_demo.git"
    LANGUAGES CXX
)
set(CMAKE_CXX_STANDARD 17)
enable_testing()

#设置变量和目录
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/bin)

set(Process_Dir ${CMAKE_SOURCE_DIR}/src/process)
set(PNC_Map_Dir ${CMAKE_SOURCE_DIR}/src/pnc_map)

#添加子目录
add_subdirectory(src)
add_subdirectory(test/map_test)
