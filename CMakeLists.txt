cmake_minimum_required(VERSION 3.17)

set(PROJECT_NAME simple-window)

project(${PROJECT_NAME})

# Needed so that cmake uses our find modules.
list(APPEND CMAKE_MODULE_PATH ${CMAKE_CURRENT_SOURCE_DIR}/cmake)

find_package(SDL2       REQUIRED)
find_package(SDL2_net   REQUIRED)
find_package(SDL2_mixer REQUIRED)
find_package(SDL2_image REQUIRED)
find_package(SDL2_gfx   REQUIRED)
find_package(SDL2_ttf   REQUIRED)


set(SOURCE_FILES
    src/main.c
    )

include_directories(src)

add_executable(${PROJECT_NAME} ${SOURCE_FILES})
target_link_libraries(${PROJECT_NAME} SDL2::Main SDL2::Net SDL2::Mixer SDL2::Image SDL2::TTF SDL2::GFX)
