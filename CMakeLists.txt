cmake_minimum_required(VERSION 3.31)
project(fmt-eigenSol VERSION 1.0.0 LANGUAGES CXX)

# add the csCMake system
include(csCMake)

cs_initialize_project(fmt-eigenSol
    # add the default configurations supported by this project, only release
    DEFAULT_CONFIG Release
)

# add libs, executables, etc
add_subdirectory(fmt-eigen)
add_subdirectory(sample)

# remember to add this at the end of the main cmake file
cs_finalize_project(fmt-eigen)
