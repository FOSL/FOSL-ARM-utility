project(FOSL-ARM-utility)

set(PROJECT_SOURCE_DIR "${PROJECT_SOURCE_DIR}/source")
set(PROJECT_BINARY_DIR "${PROJECT_BINARY_DIR}/source")

add_library(
	${PROJECT_NAME}

	${PROJECT_SOURCE_DIR}/FOSL/ARM/utility.hpp
	${PROJECT_SOURCE_DIR}/FOSL/ARM/utility.cpp
)

target_include_directories(
	${PROJECT_NAME} PUBLIC

	${PROJECT_SOURCE_DIR}
)

target_link_libraries(
	${PROJECT_NAME}

	FOSL-utility
)
