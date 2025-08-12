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

cs_install_target(fmt-eigenSample fmt-eigenSample)

cs_finalize_target(fmt-eigenSample)
