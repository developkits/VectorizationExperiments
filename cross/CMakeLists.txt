CMAKE_MINIMUM_REQUIRED(VERSION 3.0)

INCLUDE_DIRECTORIES(${CMAKE_CURRENT_SOURCE_DIR})

SET(EXECNAME CrossProduct_SERIAL)
ADD_EXECUTABLE(${EXECNAME} cross.cxx)
TARGET_INCLUDE_DIRECTORIES(${EXECNAME} PRIVATE ${VTKm_INCLUDE_DIRS})
TARGET_LINK_LIBRARIES(${EXECNAME} PRIVATE ${VTKm_LIBRARIES})
TARGET_COMPILE_OPTIONS(${EXECNAME} PRIVATE ${VTKm_COMPILE_OPTIONS})
