project(fmt-eigen LANGUAGES CXX)

# prepare standard library
cs_add_library(fmt-eigen INTERFACE)
cs_add_library(fmt-eigen::fmt-eigen ALIAS fmt-eigen)

cs_find_package(fmt-eigen PUBLIC Eigen3 REQUIRED CONFIG)
cs_find_package(fmt-eigen PUBLIC fmt REQUIRED CONFIG)

cs_target_sources(fmt-eigen
	PRIVATE_INSTALL
		fmt_eigen.h
	PRIVATE
)

cs_target_link_libraries(fmt-eigen
	INTERFACE
		Eigen3::Eigen
		fmt::fmt
		fmt-eigenSol::fmt-eigenSol_csCMakeBaseInclude
)

cs_install_target(fmt-eigen fmt-eigen DEFAULT)

cs_finalize_target(fmt-eigen)
