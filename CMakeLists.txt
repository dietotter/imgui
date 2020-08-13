cmake_minimum_required(VERSION 3.13)
project(imgui)

set(IMGUI_HEADERS
        imconfig.h
        imgui.h
        imgui_internal.h
        imstb_rectpack.h
        imstb_textedit.h
        imstb_truetype.h)

set(IMGUI_SRCS
        imgui.cpp
        imgui_demo.cpp
        imgui_draw.cpp
        imgui_widgets.cpp)

add_library(imgui STATIC ${IMGUI_SRCS} ${IMGUI_HEADERS})

#target_include_directories(imgui PUBLIC .)