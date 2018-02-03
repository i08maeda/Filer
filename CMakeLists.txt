#############################
## Compiler setting
#############################
cmake_minimum_required(VERSION 2.8)

#############################
## External libraries
#############################


#############################
## Sources
#############################
set(PROJ_SHARED_DIR ${CMAKE_SOURCE_DIR}/src)
set(PROJ_SHARED_MODEL_DIR ${PROJ_SHARED_DIR}/model)
file(GLOB PROJ_SHARED_MODEL_SOURCE ${PROJ_SHARED_MODEL_DIR}/*.cpp ${PROJ_SHARED_MODEL_DIR}/*.c)
file(GLOB PROJ_SHARED_MODEL_INCLUDE ${PROJ_SHARED_MODEL_DIR}/*.h ${PROJ_SHARED_MODEL_DIR}/*.hpp)

#############################
## Project
#############################
set(PROJ_SUB_DIR ${CMAKE_SOURCE_DIR}/proj)
add_subdirectory(${PROJ_SUB_DIR})
