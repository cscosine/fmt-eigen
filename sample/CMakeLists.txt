project(fmt-eigenSample LANGUAGES CXX)

# prepare application
cs_add_executable(fmt-eigenSample)

cs_target_sources(fmt-eigenSample
	PRIVATE
	example.cpp
)

cs_target_link_libraries(fmt-eigenSample
	PUBLIC
		fmt-eigen::fmt-eigen
)

# note: not installed on purpose - fmt-eigen is a header-only library and the
# sample is built only to validate the headers, it is not part of the install
# tree
# cs_install_target(fmt-eigenSample COMPONENT fmt-eigenSample)
