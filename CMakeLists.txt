cmake_minimum_required(VERSION 3.8)

project(git-core)

file(GLOB source_files
        "*.hpp"
        "*.cpp"
        "src/*.hpp"
        "src/*.cpp"
        "src/commands/*.hpp"
        "src/commands/*.cpp"
        "src/types/*.hpp"
        "src/types/*.cpp"
    )

add_library(${PROJECT_NAME} SHARED ${source_files})
