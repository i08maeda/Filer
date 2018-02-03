#######################################
## imageTest
#######################################
set(PROJ_NAME Filer)
project(${PROJ_NAME})

file(GLOB PROJ_SOURCE *.cpp)
file(GLOB PROJ_INCLUDE *.hpp)

include_directories(${PROJ_SHARED_MODEL_DIR})

#target_link_libraries
add_executable(${PROJ_NAME}
  ${PROJ_SOURCE} ${PROJ_INCLUDE}
  ${PROJ_SHARED_MODEL_SOURCE} ${PROJ_SHARED_MODEL_INCLUDE})

#target_link_libraries(${PROJ_NAME} ${OpenCV_LIBRARIES})
