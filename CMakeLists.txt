cmake_minimum_required(VERSION 3.5.0)
project(learngl VERSION 0.1.0 LANGUAGES C CXX)

add_executable(learngl src/main.cpp ${CMAKE_SOURCE_DIR}/include/glad.c src/shader.cpp)

link_libraries(learngl lib)

target_link_libraries(learngl PRIVATE ${CMAKE_SOURCE_DIR}/lib/glfw3.lib opengl32 gdi32)



include_directories(learngl include)