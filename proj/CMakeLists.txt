#############################
## projects
#############################

set(dir ${CMAKE_CURRENT_SOURCE_DIR})
file(GLOB subdirs RELATIVE ${dir} ${dir}/*) #このディレクトリの1階層下の全フォルダをsubdirsに相対パスで記憶

foreach(subdir ${subdirs})
  if(IS_DIRECTORY ${dir}/${subdir})
    message("subdir: ${subdir}")
    add_subdirectory(${subdir})
  endif()
endforeach()
