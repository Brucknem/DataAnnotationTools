cmake_minimum_required(VERSION 3.10)

########################################################################################################################
### Project definition ###
########################################################################################################################
project(DataAnnotationTools C CXX)
SET(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS}")
set(CMAKE_CXX_STANDARD 14)

########################################################################################################################
### Library ###
########################################################################################################################
add_subdirectory(lib)

########################################################################################################################
### Runnables ###
########################################################################################################################
add_subdirectory(standalone)

################################################################################################
### Miscellaneous ###
########################################################################################################################
add_subdirectory(misc)

########################################################################################################################
### Testing ###
########################################################################################################################
enable_testing()
add_subdirectory(test)
