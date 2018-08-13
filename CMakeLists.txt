# CMakeList.txt: vsissue-mainproject 的 CMake 项目，包括源和定义
# 此处特定于项目的逻辑。
#
cmake_minimum_required (VERSION 3.8)

add_subdirectory(thirdparty/sub)

# 将源添加到此项目的可执行文件。
add_executable (vsissuemainproject "vsissue-mainproject.cpp" "vsissue-mainproject.h")
target_link_libraries(vsissuemainproject SubProject)
# TODO: 如有需要，请添加测试并安装目标。
