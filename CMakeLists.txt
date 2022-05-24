cmake_minimum_required(VERSION 3.0.0)
project(LucyGL VERSION 0.1.0)

include(CTest)
enable_testing()

include_directories(include)

add_library(LucyGL
	"./src/OpenGL/DrawCall.cpp"
	"./src/OpenGL/FrameBuffer.cpp"
	"./src/OpenGL/IndexBuffer.cpp"
	"./src/OpenGL/Shader.cpp"
	"./src/OpenGL/Texture.cpp"
	"./src/OpenGL/Types.cpp"
	"./src/OpenGL/UniformBuffer.cpp"
	"./src/OpenGL/VertexArray.cpp"
	"./src/OpenGL/VertexBuffer.cpp"
)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
