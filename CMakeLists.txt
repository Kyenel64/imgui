cmake_minimum_required (VERSION 3.27)

project ("ImGui")

set(CMAKE_CXX_STANDARD 20)

add_library (${PROJECT_NAME} "imconfig.h" "imgui.h" "imgui.cpp" "imgui_demo.cpp" "imgui_draw.cpp"
    "imgui_internal.h" "imgui_tables.cpp" "imgui_widgets.cpp" "imstb_rectpack.h" "imstb_textedit.h"
    "imstb_truetype.h")

target_include_directories(${PROJECT_NAME} PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
