cmake_minimum_required(VERSION 3.8)
project(imgui-node-editor)

set(CMAKE_CXX_STANDARD 17) 
set(CMAKE_CXX_STANDARD_REQUIRED True)
set(CMAKE_CXX_FLAGS "-g -O3 -fPIC")

# Set our base directory
get_filename_component(IMGUI_NODE_EDITOR_ROOT_DIR ${PROJECT_SOURCE_DIR} ABSOLUTE CACHE)

# Add our project subdirectories
list(APPEND CMAKE_MODULE_PATH ${PROJECT_SOURCE_DIR}/misc/cmake-modules)
find_package(imgui REQUIRED)
find_package(imgui_node_editor REQUIRED)